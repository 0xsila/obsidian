hhhhhhhhhh , yes 

If you want good examples for SQL injection, use these : 

**Auth Bypass:** admin'; -- -        :       SELECT * FROM users WHERE username = 'admin'; -- -' AND password = 'password' 

**Boolean:** ' AND '1'='1 / ' AND '1'='2 SELECT * FROM articles WHERE author = 'admin' AND '1'='1'


Using **OR 1=1** is risky and should rarely be used in real world engagements. Since it loads all rows of the table, it may not even bypass the login, if the login expects only 1 row to be returned. Loading all rows of a table can also cause performance issues on the database. However, the real danger of **OR 1=1** is when it ends up in either an UPDATE or DELETE statement, since it will cause the modification or deletion of every row.
-- Data types : 

INT -2147483648 2147483648
BIGINT 74558888
INT(10) -- the size of the number

FLOAT 2555.444
DOUBLE 44444.66666

VARCHAR(20) -- string (size = 20)

TEXT -- many characters

DATE 2024-11-11
DATETIME 2024-11-11 11:30:00

INT(10) SIGNED
INT(10) UNSIGNED


-- Create tables : 

CREATE TABLE users(
    id INT(11) NOT NULL AUTO_INCREMENT,
	username VARCHAR(30) NOT NULL ,
    pwd VARCHAR(255) NOT NULL ,
    email VARCHAR(100) NOT NULL,
    created_at DATETIME NOT NULL DEFAULT CURRENT_TIME,
    PRIMARY KEY (id) -- have to be unique
);

CREATE TABLE comments(
    id INT(11) NOT NULL AUTO_INCREMENT,
    username VARCHAR(30) NOT NULL,
    commnet_text TEXT NOT NULL,
    created_at DATETIME NOT NULL DEFAULT CURRENT_TIME,
    users_id INT(11),
    PRIMARY KEY (id),
    FOREIGN KEY (users_id) REFERENCES users (id) ON DELETE SET NULL
);


-- insert : 
INSERT INTO users (username,pwd,email) VALUES ('0xsila','sila1999@','silayahia7@gmail.com');

-- update :
UPDATE `users` SET `id`='[value-1]',`username`='[value-2]',`pwd`='[value-3]',`email`='[value-4]',`created_at`='[value-5]' WHERE 1
UPDATE `users` SET pwd='hhhhhh' WHERE id=1 AND username='sila yahia'
UPDATE `users` SET pwd='hhhhhh' WHERE id=1 OR username='sila yahia'
--Delete : 
DELETE FROM `users` WHERE id=1
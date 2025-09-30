
nmap <ip> -p- -sC -sV -vv -oA nmap_result

interesting ports : 

139 , 445 : SMB 
6379 : Redis

redis-cli <ip> -H

GET CONFIG *
INFO

after a lot of research , we find that we can execute eval  ( EVAL lets you run Lua scripts inside Redis)

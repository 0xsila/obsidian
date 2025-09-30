### Recon : 

#### nmap : 

ssh : 22
http : 80 
http : 8080

#### web : 

nothing use

visit web at port 8080
find the version of CMS
exploit cve to get a reverse shell
user=wiki => oliver
cat /etc/wiki/........
find credentilas of oliverd
login with ssh
cat user.txt
priv esc ?
find other ports running
forward the process to our ip
port 1999 interseting
find that not work because unsupported version => cve
use the cve of ndsudo to priv esc
cat root.txt

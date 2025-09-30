### Recon : 

22 : shh
80 : http

web : 

after download file , we see the username at the url

fuzz the usernnames 

access to the files of this username
find a file
unzip the file
find a password
login with those credentials in the web
access admin panel
after analyse files , we inject a command injection in the password field 
get a reverse shell or extract the database

extract the database : 
find another username and hashed password
crack the hash

login with this credentials with ssh
cat user.txt

see what ports open : 
netstat -tulpn 2>/dev/null or ss -tulnp

we find port 8080 is open 
ssh -L 8080:127.0.0.1:8080 tobias@10.10.11.64 

goto : 127.0.0.1:8080

find a login page for a service 

try : admin and the cracked password 

we can login 

we find also the version of teh service => CVE

exploit the CVE => root

cat /root/root.txt

## Recon : 

### nmap : 

http : 80
ssh : 80

### web : 

explore the website .
find a book function .
download something .

we see .json , so it is a file => try LFI : path traversel : 

../../../../../../etc/passwd

../../../../../../proc/self/cwd/app.py  : because its a flask website , we suppose that its the source code stored here .

../../../../../../etc/hosts => dev.titanic.htb

find repositery => files ( docker )

 ../../../../../home/developer/gitea/data/gitea/gitea.db 
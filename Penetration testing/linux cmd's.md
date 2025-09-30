cat ~/.zsh_history or history (is a cmd)

id : dispaly user and group names .

uname : prints the operating sysytem 
        important for kerenl exploits 
        -a shows all information 

sudo -l : lists all cmd's you can perform as root user

id = root users are 0 , regular users start at 1000

strings : shows pritable characters in a file

ps aux : prints all running processes from all users

crontab -e

find / -name flag.txt 2>/dev/null

whereis word : locates programes

apropos keyword : find cmd's with keyword

grep -rnw / -e 'password' 2>/dev/null


enum4linux [options] ip (for smb enumeration)

-U             get userlist
-M             get machine list
-N             get namelist dump (different from -U and-M)
-S             get sharelist
-P             get password policy information
-G             get group and member list

-a             all of the above (full basic enumeration)
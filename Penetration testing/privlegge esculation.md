what is shell ? : 
-shell is a interpreter for linux cmd
-default shell in linux is zsh and it was bash

cat ~/.zsh_history or history (is a cmd)

sudo

---

### information gathering : 

**# Manual enumeration :**

whoami
id
cat /etc/passwd  |  net user
hostname
systeminfo  | uname -a  | cat /etc/issue

**# Processes : 

tasklist /SVC   |  ps aux

**# Enumerate Network info :**

find internal ports 
ipconfig /all   | ifconfig  | ip a
route print
netstat -ano  | ss -anp

**# Enumerate Firewall status and rulls :**

netsh advfirewall show allprofiles
netsh advfirewall firewall show rule name=all

iptable (linux)

**# crontab:**

schtasks /query /fo LIST /v
cat /etc/crontab

**# Enumerate readable / writable directories and files** : 

accesscheck.exe ( executable shell from microsoft)

using powershell : ( serach about it)

find / -type d -writable 2>/dev/null

**#Enumerating Unmounted Disks :**
linux : mount
windows : mountvol

**# Enumerating** **device drivers and kernel moduls**

driverquery /fo list /v       | lsmod


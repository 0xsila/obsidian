

### the file system : 

The file system used in modern versions of  Windows  is the **New Technology File System** or simply  [NTFS](https://docs.microsoft.com/en-us/windows-server/storage/file-server/ntfs-overview) .

#### The Windows\System32 Folders : 

The System32 folder holds the important files that are critical for the operating system.
the system  environment variable for the Windows directory is `%windir%` .

---

User Account Control  : is the prompt that you see to accept doing something with admin privelges

---
### CMD's : 

set : echo $PATH 
ver : operating system (OS) version
systeminfo : bayna

###### network :
`ipconfig /all` : network information
ping example.com : bayna
`tracert target_name` : bayna
nslookup: A command-line tool used to query DNS (Domain Name System) to obtain domain name or IP address mapping.

netstat : See all open connections , and more . 

###### File managment : 

cd (without parameter) : pwd

dir : ls
dir /a : ls -a
dir /s : recurssive

tree : dir + recursive dir

mkdir : 
rmdir : 
type : cat
more : for long files
copy 1.txt 2.txt : 
move 1.txt 2.txt

del or erase : rm


###### Task and process managment : 

`tasklist` : displau all the processes . 
tasklist /FI "imagename eq sshd.exe" : filter with the processe related to :  sshd.exe

taskkill /PID target_pid : to kill a process . 
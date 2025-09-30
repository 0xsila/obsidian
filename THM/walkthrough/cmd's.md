 find / -type f -not -path "/proc/*" -not -path "/sys/*" -not -path "/home/death/*" -writable 2>/dev/null

if you tipe a cmd (like nano ) in shell and its not work : try this : 
 export TERM="xterm"
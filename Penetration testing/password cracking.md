john the ripper , hashcat
hashid "hash word" : the type of hash
hashid file : kifkif

john hashfile --wordlis=path

john hashfile --show




hydra -l user -P ftp://MACHINE_IP

hydra -l <username> -P <full path to pass> 10.10.234.11 -t 4 ssh

 hydra <username> <wordlist> 10.10.234.11 http-post-form "<path>:<login_credentials>:<invalid_response>"

hydra -l <username> -P <wordlist> 10.10.234.11 http-post-form "/:username=^USER^&password=^PASS^:F=incorrect" -V
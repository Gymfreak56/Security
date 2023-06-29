used for ## WEB EXPLOITATION
```

GET / HTTP/1.1

cookie is something saved to your browser to make stuff load faster / something to make some widgets work
user agent == browser and os info(can be changed)

cURL (very powerful)

Java Script:
allows use of logic in a website

Enumeration:
robots.txt
used for web spiders

NIKTO:

BURP SUITE:

```

## Cross site scripting
```

Reflected:
non legitimate url that executes code and

Stored:
Stays on page. anyone that accesses a page will get hacked

<script>alert('HACKED');</script>


```

## WEB EXPLOITATION
```

Server-Side injection:
uses relative paths (../../../../../../../../../../../../../../../../../../../../../../../../etc/passwd)(can get usernames and /etc/hosts  for hostnames)
****DONE IN A URL*****

Malicious file upload:
you need to be able to upload a file, AND find uploaded file

Command Injection:
; == run command reguardless if command runs or npot
;whoami

```

## Demos
```

*****DONE IN A URL*****
../../../../../../../../../../../../../../../../../../../../../../../../../../../etc/passwd
/etc/hosts

<script>alert('XD')</script>

Java Script:
go to dev console
run some functions
F12==inspector

Malicious File Upload:
upload file
access file
run commands
ssh key upload

ssh keygen:
find command injection/file upload
find user
find users home dir(cat /etc/passwd)
ls -latr /var/www(home dir)
mkdir .ssh in home dir
on linops -- ssh-keygen -t rsa (use default no passphrase)
on linops -- copy entire key
echo the key and redirect into home dir/.ssh/authorized_keys

cookie stealing:
(chat room)
test for cross site scripting
make file named in cookie stealer
upload both files
use ip of website(not tunnel)


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


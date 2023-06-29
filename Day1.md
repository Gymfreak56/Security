## GRAY
```

10.50.40.121/classinfo.html

Stack Number	  Username	      Password	    lin.internet
    10	       ANME-004-M	  kA2mvZmxXvN3KFh	  10.50.29.76

GRAYHOST
username = student
pwd = password

CTFD - 10.50.20.250:8000
ANME-004-M
ANME-004-M

```

## Pen Testing
```  

Virtual and Physical
***TAKE NOTES***

Phase2:

Phase3: Footprinting

Phase4: Exploiting and Initial Access

Phase5: 

Phase6: Document Mission

OPNOTES -- Notes taken while on mission (CAN BE PUBLISHED)
REPORT -- Analized (put into a bigger picture)

REPORTS:
EXECUTIVE Summary: Dumbed down
TECHNICAL Summary: Includes technical information

Things to report:
Depends on the mission

```

## Scanning and Recon
```

OPEN SOURCE:


DOCUMENTATION:
DOCUMENT YOUR STUFF

DATA TO COLLECT:
Collect what youre told to collect

HTML:
Know kinda how to read it

SCANNING:
Don't scan till you do passive recon
1. HOST DISCOVERY(Find hosts that are online)(Ping)
2. PORT ENUMERATION(NMAP)(PATTERNS)
3. PORT INTERROGATION(NETCAT)(BANNER GRAB)

NMAP Scripting Engine:


```

## Vulnerability Research
```

OBJ:
Understand initial access

Initial Access:
Phishing EMAILS -- Most Common
Critential Reuse -- SAVE CRIDENTIALS


EXPLOIT RESEARCH:
Transition into weaponization
Vulnerability -- Specific circumstances bad stuff can happen
Exploits -- Someone made code to use that vulnerability

Research:
Open source
Organizational Capabilities

Capabilities:
Collection -- Collecting data
Effects -- Changing something

TESTING:
TEST YOUR STUFF

PLAN:
HAVE A PLAN

```

## NOTES
```

##HOST DISCOVERY
for i {1..254}; do (ping -c1 192.168.28.$i | grep "bytes from" &); done

## PORT DISCOVERY
#nmap -Pn -T4 --minrate=8675309 -sT 192.168.28.1 -p22,80
## add --script as needed. MINRATE OPTIONAL

## PORT INTERROGATION
#nc 192.168.28.1 22
#*press enter*

```

## NMAP SCRIPTS
```

nmap -Pn -T4 -sT 10.50.27.129 -p80 --script=http-enum (grabs defaults)
nmap -Pn -T4 -sT 10.50.27.129 -p80  --script=http-robots.txt (gives you an idea of what file is)
nmap -Pn -T4 -sT 10.50.27.129 -p445 --script=smb-os-discovery (gives smb info)

```

## Control Sockets
```

Original term
-M == master
-S == slave

NEW TERM
-M == multiplexing
-S == socket

ssh -MS /tmp/gray 10.50.29.76 (saves it in a file called gray)

ssh -S /tmp/gray dummy (dummy == placeholder)

ssh -S /tmp/gray dummy -O forward -L 1111:192.168.28.111:80
ssh -S /tmp/gray dummy -O forward -L 1112:192.168.28.111:8080

ssh -S /tmp/gray dummy -O cancel -L 1111:192.168.28.111:80
ssh -S /tmp/gray dummy -O cancel -L 1112:192.168.28.111:8080

ssh -S /tmp/gray dummy -O forward -D 9050 (scan)
ssh -S /tmp/gray dummy -O cancel -D 9050 (close)



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


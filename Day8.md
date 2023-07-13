## Windows Access Control Mode
```

Access token:
SID
  Security descriptors:
  DACL
  SACL
  ACEs

```

## Dynamic Link Library(DLL) Search Order
```

HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Session Manager\KnownDLLs
The directory the the Application was run from
The directory specified in in the C+ function GetSystemDirectory()
The directory specified in the C+ function GetWindowsDirectory()
The current directory

```

## Windows Intergrity Mechanism
```

Used for applications

```

## UAC(User Account Control)
```

Asks for permissions when trying to preform changes to the computer
reg query HKLM\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System

```

## Auto Elevate Executables
```

Requested Execution Levels:
asinvoker
highestAvailable

```

## Scheduled Tasks/Services
```

Write Permissions
Non-Standard Locations
Unquoted Executable Paths
Vulnerabilities in Executables
Permissions to Run As SYSTEM

schtasks /query /fo LIST /v

wmic service list full
sc query

```

## DLL Hijacking
```

Identify Vulnerability
Take advantage of the default search order for DLLS
NAME_NOT_FOUND present in executable’s system calls
Validate permissions
Create and transfer Malicious DLL

```

## Vulnerable Services
```

Identify Vulnerability
Validate permissions
Validate Executable Paths
Replace with Malicious File

```

## Persistence
```

Survives:
Reboots
Credential changes
DHCP IP reassignment
Etc.

Considerations include:
File naming
File location
Timestomping
Port selection

```

## Covering Tracks
```

auditpol /get /category:* | findstr /i "success failure"

Event IDS:
4624/4625 -- Successful/failed login

4720 -- Account created

4672 -- Administrative user logged on

7045 -- Service created

Event Logs:
c:\windows\system32\config\
File-Type: .evtx/.evt

```

## DEMO 
```

Start Procmon
start vulnerable service
filter on process name / result contains NAME NOT FOUND / path contains dll
SSP.....dll
msfvenom -p windows/exec CMD='cmd.exe /C "whoami" > C:\' -f dll > SSPICLI.dll
scp file to windows station


```

## 
```



```

## 
```



```


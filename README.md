#IOS Project 1
##A shell script to view and filter apache logs.

POSIXly correct
Works in: Linux, FreeBSD
Should work in: MacOS

Flags:
```
-a YYYY-MM-DD HH:MM:SS  - Search after date
-b YYYY-MM-DD HH:MM:SS  - Search before date
-ip IPv4|IPv6           - Search IP
-uri URI                - Search URI
```

Commands:
```
list-ip
list-host
list-uri
hist-ip    - Creates histogram of IPs
hist-load  - Creates histogram of load
```

Usage:
```
./wana [filter flags - OPTIONAL] [command] [log [log2 [...]]]
```
Example:
```
./wana -a 2019-02-15 -b 2019-02-20 list-hosts log1 log2 log3
```
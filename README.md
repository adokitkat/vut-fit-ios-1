# IOS Project 1

## A shell script to view and filter apache logs.

Prints result to STDOUT. 

POSIX-ly correct

Works on: Linux, FreeBSD

Should work on: MacOS

Flags:
```
-a YYYY-MM-DD HH:MM:SS  - Find entries after date
-b YYYY-MM-DD HH:MM:SS  - Find entries before date
-ip IPv4|IPv6           - Find by specified IP
-uri URI                - Find by specified URI
```

Commands:
```
list-ip    - Lists IPs
list-host  - Lists hosts
list-uri   - Lists URIs
hist-ip    - Creates histogram of IPs
hist-load  - Creates histogram of load
```

Usage:
```
./wana [filter flags - OPTIONAL] [command - OPTIONAL] [log [log2 [...]] - When no log is provided, reads from STDIN]
```
Example:
```
./wana -a 2019-02-15 -b 2019-02-20 list-hosts log1 log2 log3
```

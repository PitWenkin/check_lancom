# Check LANCOM
Nagios/Icinga script to check availability of access points managed by a LANCOM wlan controller

Used to check LANCOM WLAN Controllers https://www.lancom-systems.com

# Usage:
```
  ./check_lancom -h [hostname] -c [community] -p [port] -W [warning] -C [critical]
```

# Options:
```
  -h [hostname]
  -c [SNMPv2 community name]	(default is public)
  -p [port]			(default is 161)
  -t [timeout]  (default is 10 seconds)
  -W [warning]  Percentage of accesspoints which have to be down to return a warning message (default is 1)
  -C [critical] Percentage of accesspoints which have to be down to return a critical message (default is 10)
```

# Examples:
```
  ./check_lancom -h 1.2.3.4 -c public 
  ./check_lancom -h 1.2.3.4 -p 4321 -c public -t 30
```

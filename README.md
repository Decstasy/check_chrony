# check_chrony
Icinga2 / Nagios check for Chrony NTP &amp; PTP offset to reference.
Performance data is also included and no sudo privileges are needed for execution.

## Example
```bash
user@server:~$ ./check_chrony -w 1 -c 3
OK: Time offset of +0.000056025 seconds to reference. | offset=+0.000056025s;1;3
```
-x Seconds: Your client is running x seconds slower than the reference.  
+x Seconds: ... Guess ^^

## Requirements
Perl min. version 5.10.1

## Tested on
* Ubuntu 16.04
* Ubuntu 18.04
* Debian 9

# Parameters
* -w [Warning threshold] :  in seconds (e.g. 2 or 0.4)
* -c [Critical threshold] : in seconds (e.g. 4 or 0.8)
* -h : Help

# Notes
Full documentation will follow soon.

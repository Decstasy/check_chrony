# check_chrony
Icinga2 / Nagios check for Chrony NTP &amp; PTP offset to reference.
Performance data is also included and no sudo privileges are required for execution.

## Example
```bash
user@server:~$ ./check_chrony -w 1 -c 3
OK: Time offset of +0.000056025 seconds to reference. | offset=+0.000056025s;1;3
```
-x Seconds: Your client is running x seconds slower than the reference.  
+x Seconds: ... Guess ^^

## Requirements
Perl min. version 5.10.1

### Tested on
* Ubuntu 16.04 - 22.04 LTS
* Debian 9 - 11
* CentOS 7,8, Stream
* RHEL 7 - 9
* Alma 9
* Arch

### Parameters
* -w [Warning threshold] : (required) in seconds (e.g. 2 or 0.4)
* -c [Critical threshold] : (required) in seconds (e.g. 4 or 0.8)
* -h : Help

## Notes
Full documentation will follow soon.

## License
This program is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.

This program is distributed hoping that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program; if not, see http://www.gnu.org/licenses/

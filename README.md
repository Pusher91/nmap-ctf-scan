# nmap-ctf-scan
Simple nmap bash script to scan ctf boxes.



```console
./script.sh <target>
Target: (target)

Scanning scan: sudo nmap (target) -p- -oN ping-scan --min-rate 1000

Starting Nmap 7.92 ( https://nmap.org ) at 2022-07-11 17:50 CDT
(nmap scan output)
Nmap done: 1 IP address (1 host up) scanned in 147.57 seconds
Scan finished.
Open ports: (list of open ports of ./ping-scan)

Running scan: sudo nmap 10.129.223.201 -p(list of open ports of ./ping-scan) -sV -sC -oN script-scan

Starting Nmap 7.92 ( https://nmap.org ) at 2022-07-11 17:53 CDT
(nmap scan output)
Nmap done: 1 IP address (1 host up) scanned in 194.46 seconds
-sV -sC again open ports finished.

Running UDP scan: sudo nmap 10.129.223.201 -sU -oN udp-scanStarting Nmap 7.92 ( https://nmap.org ) at 2022-07-11 17:56 CDT
Nmap scan report for 10.129.223.201
(nmap scan output)
Nmap done: 1 IP address (1 host up) scanned in 26.06 seconds
UDP scan finished.```

```console
./script.sh 10.129.223.201
Target: 10.129.223.201

Skipping -p- scan.  File ./ping-scan already exists.
Skipping -sV -sC -p<open ports from ./ping-scan>.  The file ./script-scan already exists.
Skipping -sU scan.  The file ./udp-scan already exists.```

# nmap-ctf-scan
Simple nmap bash script to scan ctf boxes.



```console
nmap-ctf-scan 10.129.223.201
### Target: 10.129.223.201 ###

### Running scan: sudo nmap 10.129.223.201 -p- -oN ping-scan --min-rate 1000 ###
Starting Nmap 7.92 ( https://nmap.org ) at 2022-07-12 08:48 CDT

(nmap scan output)

Nmap done: 1 IP address (1 host up) scanned in 112.97 seconds
### Scan finished. ###
### Open ports: 53,80,88,135,139,389,445,464,593,636,1433,3268,3269,4411,5985,9389,49667,49673,49674,49700,49704,53138, ###

### Running scan: sudo nmap 10.129.223.201 -p53,80,88,135,139,389,445,464,593,636,1433,3268,3269,4411,5985,9389,49667,49673,49674,49700,49704,53138, -sV -sC -oN script-scan ###

Starting Nmap 7.92 ( https://nmap.org ) at 2022-07-12 08:50 CDT

(nmap scan output)

Nmap done: 1 IP address (1 host up) scanned in 194.36 seconds
### -sV -sC again open ports finished. ###

### Running scan: sudo nmap 10.129.223.201 -sU -oN udp-scan ###
Starting Nmap 7.92 ( https://nmap.org ) at 2022-07-12 08:53 CDT

(nmap scan output)

Nmap done: 1 IP address (1 host up) scanned in 10.57 seconds
### UDP scan finished. ###
```

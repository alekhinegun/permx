## Basic Recon

### 

Create the ip address variable

```bash
ip=10.129.95.125
```

Perform a basic scan on the ports to observe any opne ports.

```bash
nmap -p- $ip
```

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-12-02 12:49 CST
Nmap scan report for 10.129.95.125
Host is up (0.077s latency).
Not shown: 65533 closed tcp ports (reset)
PORT   STATE SERVICE
22/tcp open  ssh
80/tcp open  http

Nmap done: 1 IP address (1 host up) scanned in 42.14 seconds


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

![nmapportscan](https://github.com/user-attachments/assets/6cfab490-88ef-4185-8dc4-3d8c36f12e31)

```bash
nmap -p22,80 $ip -A
```
![image](https://github.com/user-attachments/assets/201bf43e-7e59-499c-8409-98e8aaf8a2a9)

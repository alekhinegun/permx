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


```bash
sudo vim /etc/hosts
```
![image](https://github.com/user-attachments/assets/2ed9b810-a00a-4cf0-9574-d8dd5bd1f357)

```bash
nmap -p22,80 $ip -A
```

![image](https://github.com/user-attachments/assets/35625c54-68cb-4b02-9c29-e098b41d0aa2)
## Initial Hunch
After going to the webpage I observe
![image](https://github.com/user-attachments/assets/53309791-d3e1-4f00-90db-8f1344529aec)

```bash
dirb http://permx.htb
```

```bash
feroxbuster --url http://permx.htb
```

![image](https://github.com/user-attachments/assets/2f72a185-d0d6-4e4b-95eb-31ceaa84aed3)

![image](https://github.com/user-attachments/assets/db00849a-bc87-4572-a3cb-8340bfdc74b8)
```bash
ffuf -u http://permx.htb -H "Host:FUZZ.permx.htb" -w /usr/share/seclists/Discovery/DNS/subdomains-top1million-20000.txt -fw 18
```

![image](https://github.com/user-attachments/assets/64a2504c-a5e2-4e49-9391-618ce6b02e0e)

![image](https://github.com/user-attachments/assets/7d7642d2-817a-48cb-b189-ec10b837ade3)


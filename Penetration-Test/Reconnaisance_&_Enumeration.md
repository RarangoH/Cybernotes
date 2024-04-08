# Scanning 


[IP Scanning](#IP-Scanning)

[Port Scanning](#Port-Scan)

## IP-Scanning
#### Tools: 
- <strong>netdiscover</strong>

- <strong>arp-scan</strong>

    

## Port-Scan
#### Tools:
- <strong>nmap</strong>

        nmap -sC -sV <Target_IP>
        nmap -p- <Target_IP> --> recommended to run in the background to discard more ports
nmap Flags: [-p- : scans all ports] [-sC : ] [-A : agressive ] [-sV : service Version] [-sU : UDP scan]
- <strong>rustscan</strong> 
- <strong>auto</strong>
- <strong>autorecon - automated tool</strong>
- <strong>proxychains</strong>
        
        

Port 22 - SSH
Tools:
    
    ssh-audit

SMB

    smbclient -N -L \\\\TargetIP\\ --> (-N : means null session, no password / -L : lists all of the shares)
    smbclient -N \\\\TargetIP\\shareName --> (tries to connect to the share)


DNS zone transfer attack

attack asks dns server to give all entries for particualar zone (particular IP) test.com needs to be replaced for dns server

dig axfr test.com @IP


RDP

xfreerdp /u:user /p:"password" /v:IP

Enumerating WordPress: wpscan

HTTP 

    Directories
    Tool : gobuster
    gobuster dir -t20 --wordlist wordlist.txt -u http://ip -x -aspx

    gobuster vhost --wordlist wordlist.txt -u http:/IP  --exclude-length 334

    -x flag searchs for only a file extension needed.
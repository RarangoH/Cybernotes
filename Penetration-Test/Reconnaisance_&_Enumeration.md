# Scanning 


[IP Scanning](#IP-Scanning)

[Port Scanning](#Port-Scan)

### IP-Scanning
Tools: 

    netdiscover

    arp-scan

### Port-Scan
Tools:

        nmap
        rustscan
        auto
        autorecon - automated tool

Port 22 - SSH
Tools:
    
    ssh-audit

SMB

    smbclient -N -L \\\\TargetIP\\ --> (-N : means null session, no password / -L : lists all of the shares)
    smbclient -N \\\\TargetIP\\shareName --> (tries to connect to the share)
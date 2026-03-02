# Reconnaissance Phase

## Tool Used
Nmap

## Command
nmap -v -sS -A -T4 10.0.2.5

## Key Findings

Multiple open services were detected:

- FTP (vsftpd 2.3.4)
- SSH (OpenSSH 4.7)
- HTTP (Apache 2.2.8)
- MySQL
- PostgreSQL
- Samba
- VNC
- IRC

## Observations

Several outdated services were identified,
indicating potential security vulnerabilities.

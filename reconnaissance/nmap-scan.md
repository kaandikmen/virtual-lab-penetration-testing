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

# Reconnaissance Phase

## Objective
To identify open ports, running services, and operating system details
on the target virtual machine.

## Tool Used
Nmap (Network Mapper)

## Command Executed

nmap -v -sS -A -T4 10.0.2.5

## Scan Explanation

- -sS → TCP SYN Scan (Stealth Scan)
- -A → OS detection, version detection, script scanning
- -T4 → Faster scan timing

## Key Findings

The scan revealed multiple open services:

| Port | Service | Version |
|------|---------|----------|
| 21   | FTP     | vsftpd 2.3.4 |
| 22   | SSH     | OpenSSH 4.7 |
| 23   | Telnet  | telnetd |
| 80   | HTTP    | Apache 2.2.8 |
| 3306 | MySQL   | 5.0.51 |
| 5432 | PostgreSQL | 8.3 |
| 139/445 | Samba | 3.0.20 |
| 5900 | VNC     | 3.3 |

## Security Observations

- Several services are outdated.
- Anonymous FTP login was enabled.
- Samba version is known to contain vulnerabilities.
- Telnet service exposes unencrypted communication.

## Conclusion

The target system exposes multiple high-risk services,
indicating poor security configuration.

## Scan Output Screenshot

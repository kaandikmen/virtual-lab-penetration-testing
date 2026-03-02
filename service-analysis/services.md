# Service Analysis

## Overview

After performing reconnaissance, multiple outdated and potentially vulnerable services were identified.

---

## FTP (vsftpd 2.3.4)

- Anonymous login enabled
- Known historical vulnerabilities exist for this version

Risk:
Unauthorized file access and potential remote code execution.

---

## SSH (OpenSSH 4.7)

- Old version detected

Risk:
Brute-force attacks and possible version-based exploits.

---

## Telnet

- Unencrypted communication protocol

Risk:
Credentials can be intercepted via packet sniffing.

---

## Samba (3.0.20)

- Outdated version

Risk:
Remote code execution vulnerabilities and unauthorized access.

---

## MySQL / PostgreSQL

- Database services exposed to network

Risk:
Weak credentials or misconfiguration may lead to database compromise.

---

## VNC

- Remote desktop service exposed

Risk:
Unauthorized remote control if authentication is weak.

---

## Security Summary

The system shows multiple critical misconfigurations and outdated services,
making it highly vulnerable in a real-world scenario.

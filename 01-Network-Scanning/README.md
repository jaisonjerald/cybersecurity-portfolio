# 🔍 Network Scanning with Nmap

## Project Overview

This project demonstrates the use of **Nmap (Network Mapper)** to discover hosts, identify open ports, detect services, and gather information about a target system in a controlled lab environment.

> **Disclaimer:** All scans in this repository were performed in a personal lab or on systems where I had permission to test. Do not scan networks or systems without authorization.

---

## Objectives

- Discover live hosts
- Identify open TCP ports
- Detect running services
- Identify operating systems
- Perform version detection
- Understand basic network reconnaissance

---

## Lab Environment

| Component | Details |
|-----------|---------|
| OS | Kali Linux |
| Tool | Nmap |
| Target | Metasploitable 2 (Lab VM) |
| Network | VirtualBox Host-Only |

---

## Nmap Commands Used

### Host Discovery

```bash
nmap -sn 192.168.56.0/24
```

### TCP SYN Scan

```bash
nmap -sS 192.168.56.101
```

### Service Version Detection

```bash
nmap -sV 192.168.56.101
```

### Operating System Detection

```bash
nmap -O 192.168.56.101
```

### Aggressive Scan

```bash
nmap -A 192.168.56.101
```

---

## Sample Findings

| Port | Service | Status |
|------|---------|--------|
| 21 | FTP | Open |
| 22 | SSH | Open |
| 23 | Telnet | Open |
| 80 | HTTP | Open |
| 3306 | MySQL | Open |

---

## Security Recommendations

- Disable unused services.
- Restrict access using firewall rules.
- Keep operating systems and applications patched.
- Use strong authentication.
- Continuously monitor exposed services.

---

## Skills Demonstrated

- Network Reconnaissance
- Port Scanning
- Service Enumeration
- Operating System Detection
- Network Security Assessment

---

## Tools

- Kali Linux
- Nmap
- VirtualBox
- Metasploitable 2

---

## Screenshots

Screenshots of command execution and scan results will be added to the `images/` folder.

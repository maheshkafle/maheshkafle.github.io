# 🔍 Essential Nmap Commands for Network Scanning

Nmap (Network Mapper) is one of the most powerful tools used in cybersecurity for network discovery and security auditing.  
This guide covers essential Nmap commands every beginner should know.

---

## 1. 🖥️ Basic Host Discovery

Scans a single host to check if it is up and identifies open ports.  
Useful for quick host checks.

```bash
nmap 192.168.1.10

---

## 2. 🖥️ Scan an Entire Subnet

Discovers all live hosts and open ports in a network range.
Useful for network mapping.

```bash
Command: nmap 192.168.1.0/24

---

## 3. 🖥️ **Service & Version Detection**

Identifies running services and their versions.
Helps in vulnerability assessment.

```bash
Command: nmap -sV 192.168.1.10

---

## 4. 🖥️ OS Detection

Attempts to determine the target's operating system.
Useful for profiling hosts.

```bash
Command: nmap -O 192.168.1.10

---

## 5. 🖥️ Aggressive Scan

Performs OS detection, version detection, scripts, and traceroute.
Deep enumeration.

```bash
Command: nmap -A 192.168.1.10

---

## 6. 🖥️ Scan Specific Ports

Targets only selected ports instead of scanning all.
Useful for focused testing.

```bash
Command: nmap -p 22,80,443 192.168.1.10

---

## 7. 🖥️  Scan Top 100 Ports

Fast scan focusing on the most commonly used ports.
Useful for quick assessments.

```bash
Command: nmap --top-ports 100 192.168.1.10

---

## 8. 🖥️ Stealth SYN Scan

Performs a half-open scan that avoids full TCP handshakes.
Useful for stealthy scanning.

```bash
Command: nmap -sS 192.168.1.10

---

## 9. 🖥️ UDP Scan

Checks for UDP services such as DNS, DHCP, and SNMP.
Useful for full coverage.

```bash
Command: nmap -sU 192.168.1.10

---

## 10. 🖥️ Vulnerability Scan (NSE)

Uses Nmap Scripting Engine to detect common vulnerabilities.
Useful for security audits.

```bash
Command: nmap --script vuln 192.168.1.10

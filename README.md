# nmap-recon-project
A simple and professional project using Nmap for cybersecurity
# 🔍 Nmap Reconnaissance Project

This project demonstrates the use of the Nmap tool for basic network reconnaissance. It includes scanning a target IP to identify open ports, services, and their versions.

---

## 🎯 Objective

To simulate a real-world ethical hacking task by performing a service and port scan using Nmap and documenting the results. This project showcases hands-on cybersecurity skills relevant for vulnerability assessment roles.

---

## 📂 Project Structure


nmap-recon/
├── README.md               → This documentation file
├── scripts/
│   └── full_scan.sh        → Nmap scan shell script
└── reports/
    └── scan_report.txt     → Output of Nmap command


---

## ⚙ Nmap Command Used

bash
nmap -sV -p- 10.156.59.200


- -sV : Attempts to determine service/version info.
- -p- : Scans all 65535 TCP ports.

---

## 📁 Script (scripts/full_scan.sh)

bash
#!/bin/bash

TARGET="10.156.59.200"
OUTPUT="reports/scan_report.txt"

echo "[*] Scanning $TARGET..."
nmap -sV -p- $TARGET -oN $OUTPUT
echo "[+] Scan complete. Results saved to $OUTPUT"


---

## 📊 Sample Output (reports/scan_report.txt)


PORT   STATE SERVICE VERSION
53/tcp open  domain  dnsmasq 2.51
MAC Address: 06:A0:04:25:27:05 (Unknown)


---

## ✅ Skills Demonstrated

- Network scanning with Nmap  
- Port and service enumeration  
- Writing and executing Bash scripts  
- Saving and organizing recon reports  
- Git & GitHub for version control and showcasing work

---

## 📌 Notes

> This simulation was conducted in a *controlled lab environment* using test devices and IPs under permission. No real-world systems were harmed or targeted.

---

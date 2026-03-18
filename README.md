# 🔍 Nmap Network Exposure Analysis – Cybersecurity Internship Task 1

> **Short Description:**  
>  
> This project documents a network scan performed with Nmap to identify active devices, detect open ports, and analyze potential security risks from exposed services in a local network environment.

---

## ✅ Objective

Perform a local network scan using Nmap, identify active devices, detect open TCP ports, and analyze potential security risks based on exposed services.

---

## 🛠️ Tools & Configuration

- **Tool Used:** Nmap
- **Scan Type:** SYN Scan (`-sS`)
- **IP Range Scanned:** 192.168.1.0/24

---

## 📊 Scan Results

The following open ports were discovered across the scanned IP range:

| Port | Service | Risk Description |
|------|---------|------------------|
| **22** | SSH | Common target for brute-force attacks |
| **80** | HTTP | Might expose outdated or unpatched web applications |
| **443** | HTTPS | Ensure SSL certificates are valid and properly configured |
| **3306** | MySQL | Direct exposure of databases poses a high risk |

---

## 🔍 Analysis & Findings

- Open ports indicate services actively listening for connections on the network.
- Services like SSH and MySQL, if exposed and unprotected, significantly increase the attack surface.
- Weak or default configurations are vulnerable to exploitation through automated tools.

---

## 🔐 Security Implications

- **SSH (Port 22):** Restrict access to specific trusted IP addresses or disable if not required.
- **HTTP (Port 80):** Regularly patch and secure web applications to avoid vulnerabilities.
- **MySQL (Port 3306):** Databases should never be directly exposed to the internet without strict security controls.
- **General Advice:** Regularly audit open ports and disable unnecessary services to reduce risk.

---

## 📌 Conclusion

Using Nmap for network scanning is crucial for identifying open services and potential exposures. This task provided valuable insights into how attackers might exploit misconfigured or unnecessary services and emphasized the importance of proactive network security management.

---

## 📁 Files Included

- `README.md` – Full report and analysis
- `code.html` – HTML version of the scan report

---
## 🔗 About

This repository contains the results and analysis of a network scan performed using Nmap on a local IP range. The scan identified active devices and their open TCP ports using a SYN scan. The report lists common services running on these ports and highlights potential security risks, such as exposed vulnerable services that could be exploited.

---

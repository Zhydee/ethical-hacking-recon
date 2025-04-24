## 🛡️ Ethical Hacking – Reconnaissance Phase</h2>

<p>This repository documents the reconnaissance phase of a penetration test conducted on a demo web application: <a href="http://megamegapom.free.nf/" target="_blank">megamegapom.free.nf</a>, as part of an Ethical Hacking coursework group project (NWC4233).</p>

<h3>👨‍💻 Project Author:</h3>
<ul>
  <li><strong>Name:</strong> Muhammad Zaidi Fahmi Bin Zainudin</li>
  <li><strong>Student ID:</strong> AM2311015290</li>
  <li><strong>Tools Used:</strong> nslookup, WhatWeb, Nmap, OpenSSL</li>
  <li><strong>Platform:</strong> Kali Linux VM</li>
</ul>

<h3>🔍 Objectives</h3>
<ul>
  <li>Perform passive and active reconnaissance on the target system</li>
  <li>Identify exposed technologies, DNS configurations, and open ports</li>
  <li>Analyze vulnerabilities and suggest countermeasures</li>
</ul>

## 🔍 Reconnaissance Summary

### 🧾 DNS Enumeration (nslookup)
- IP resolved: `185.27.134.163`
- Nameserver: `ns1.infinityfree.com`
- Hosting provider: iFastNet LTD (shared hosting)
- Zone transfers: Blocked/restricted

### 🌐 Web Tech Fingerprinting (WhatWeb)
- Detected server: `OpenResty` (built on nginx)
- Client-side tech: JavaScript
- Server location: United Kingdom

### 🚪 Port Scanning (Nmap)
- Open ports: 80 (HTTP), 443 (HTTPS)
- Services: `tcpwrapped` (suggesting firewall or wrapper protection)
- Firewall detected via filtered responses

### 🔐 SSL/TLS Check (OpenSSL)
- TLS handshake failed
- No certificate presented
- Likely misconfigured or restrictive SSL stack

## 📁 Repository Structure
```
/report/         → Full technical report (PDF)
/screenshots/    → Output screenshots by tool (grouped by tool)
/project_info/   → Original project brief (assignment question)
/tools_used.md   → Summary of tools used
README.md        → This file
```
## 📸 Screenshots Preview

All tool output screenshots are stored in the `/screenshots/` folder, categorized by tool:
- `nslookup/` – DNS resolution, SOA queries
- `whatweb/` – Technology fingerprinting
- `nmap/` – Port scanning

---
<h2>🛡️ Suggested Countermeasures</h2>
<ul>
  <li>Restrict DNS Zone Transfers</li>
  <li>Remove or mask HTTP headers (e.g., Server: OpenResty)</li>
  <li>Close unused ports and restrict access via firewall</li>
  <li>Fix SSL/TLS configuration, enforce TLS 1.2/1.3 with valid certs</li>
</ul>

## 📋 Project Question

The original project brief for this penetration testing assignment is available [here](https://github.com/Zhydee/ethical-hacking-recon/tree/main/project_info).

<h2>📄 Full Report</h2>
<p>You can find the full PDF version of the technical report <a href="https://github.com/Zhydee/ethical-hacking-recon/tree/main/report">here</a>.</p>

<h2>📌 Notes</h2>
<p>This project was conducted under ethical hacking guidelines and for educational purposes only. No actual intrusion or alteration was performed on the live system.</p>

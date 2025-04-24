# 🧰 Tools Used in Reconnaissance Phase

### 1. `nslookup`
- Purpose: Resolve domain name to IP and check DNS records.
- Use Case: Basic DNS footprinting and infrastructure mapping.

### 2. `WhatWeb`
- Purpose: Identify web technologies from HTTP responses.
- Use Case: Determine backend platform and frameworks in use.

### 3. `Nmap`
- Purpose: Port scanning and service detection.
- Flags used:
  - `-sS`: Stealth scan
  - `-sV`: Service version detection
- Use Case: Enumerate open ports and analyze defensive measures.

### 4. `OpenSSL`
- Purpose: Test SSL/TLS handshake for misconfigurations.
- Command: `openssl s_client -connect megamegapom.free.nf:443`
- Use Case: Check for certificate issues or insecure cipher support.

### Optional Tools (Not used but recommended)
- `theHarvester`
- `whois`
- `crt.sh`
- `wafw00f`


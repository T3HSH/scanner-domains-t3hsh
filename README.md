# 🛡️ Cloudflare IP & Domain Scanner

**A powerful Cloudflare IP & Domain Scanner built for penetration testing, reconnaissance, and Cloudflare Worker configurations.**

---

## 🚀 Overview

**Cloudflare IP & Domain Scanner** is a lightweight yet powerful reconnaissance tool designed for scanning **Cloudflare-protected domains and IP addresses**.

Unlike traditional scanners, this project focuses specifically on Cloudflare environments, providing detailed information about:

* Open ports
* Running services
* DNS records
* SSL/TLS configuration
* Cloudflare detection
* Security information
* Network details

It is fully compatible with **Cloudflare Worker configurations** and delivers clean, structured reports for security analysis.

> ⚡ Simply provide a target domain or IP address and let the scanner do the rest.

---

# ✨ Features

* 🔍 Fast Port Scanning
* 🌐 DNS & Domain Analysis
* ☁️ Cloudflare Detection
* 🔒 SSL / TLS Validation
* 🛡️ Security Information
* 📍 ASN & Geo Location Lookup
* 📊 Clean JSON Reports
* ⚙️ Full Cloudflare Worker Support
* 🎯 Smart Target Detection

---

# 📦 Installation

```bash
git clone https://github.com/T3HSH/cloudflare-scanner.git

cd cloudflare-scanner

pip install -r requirements.txt
```

---

# 🚀 Usage

```bash
python scanner.py -t example.com
```

### Full Scan

```bash
python scanner.py -t example.com --full
```

### Save Report

```bash
python scanner.py -t example.com -o report.json
```

### Worker Mode

```bash
python scanner.py -t worker.example.com --worker
```

---

# ⚙️ Command Line Arguments

| Parameter        | Description                               |
| ---------------- | ----------------------------------------- |
| `-t`, `--target` | Target domain or IP address               |
| `-p`, `--ports`  | Port range (Example: `1-1000`)            |
| `-f`, `--full`   | Full scan with additional security checks |
| `-o`, `--output` | Save output to a file                     |
| `-w`, `--worker` | Cloudflare Worker scanning mode           |

---

# 📋 Example Output

```text
🎯 TARGET LOCKED
────────────────────────────────────

Domain        : example.com
IP Address    : 185.199.108.153
Cloudflare    : YES ☁️
Status        : LIVE
Open Ports    : 80, 443, 22, 53
SSL / TLS     : Valid
Server        : cloudflare
ASN           : AS13335 Cloudflare, Inc.
Location      : Europe 🇩🇪 Germany

────────────────────────────────────
✅ Report saved → report.json
```

---

# 🎯 Designed For

* Cloudflare Domains
* Cloudflare Protected Servers
* Cloudflare Workers
* Security Reconnaissance
* Network Analysis
* Penetration Testing

---

# ⚠️ Disclaimer

This project is intended **only for authorized security testing and educational purposes**.

Only scan systems and domains that you own or have explicit permission to assess. The author is **not responsible for any misuse** of this software.

---

# 📜 License

This project is licensed under the **MIT License**.

See the **LICENSE** file for more information.

---

# ❤️ Author

Developed with ❤️ by **T3HSH**

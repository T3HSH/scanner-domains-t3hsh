<p align="center">

🌍 **Language**

🇺🇸 **English** | <a href="./README_FA.md">🇮🇷 فارسی</a>

</p>

# 🛡️ Cloudflare IP & Domain Scanner

**A powerful scanner for Cloudflare-protected domains and IP addresses, designed for reconnaissance, analysis, and Cloudflare Worker environments.**

---

# 🚀 Overview

**Cloudflare IP & Domain Scanner** is a lightweight yet powerful reconnaissance tool built specifically for scanning **Cloudflare-protected domains and IP addresses**.

Unlike traditional scanners, this project focuses on Cloudflare environments and provides detailed information including:

* Open ports
* Running services
* DNS records
* SSL/TLS configuration
* Cloudflare detection
* Security information
* Network details

The scanner is fully compatible with **Cloudflare Worker configurations** and generates clean, structured reports for security analysis.

> ⚡ Simply provide a target domain or IP address, and the scanner will handle the rest.

---

# ✨ Features

* 🔍 Fast Port Scanning
* 🌐 DNS & Domain Analysis
* ☁️ Cloudflare Detection
* 🔒 SSL / TLS Validation
* 🛡️ Security Information
* 📍 ASN & Geo Location Lookup
* 📊 Clean & Structured Reports
* ⚙️ Full Cloudflare Worker Support
* 🎯 Smart Target Detection

---

# 🚀 Usage

### Basic Scan

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

| Parameter        | Description                                         |
| ---------------- | --------------------------------------------------- |
| `-t`, `--target` | Target domain or IP address                         |
| `-p`, `--ports`  | Port range (e.g. `1-1000`)                          |
| `-f`, `--full`   | Perform a full scan with additional security checks |
| `-o`, `--output` | Save the report to a file                           |
| `-w`, `--worker` | Enable Cloudflare Worker scanning mode              |

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

* Cloudflare-Protected Domains
* Cloudflare-Protected Servers
* Cloudflare Workers
* Security Reconnaissance
* Network Analysis
* Authorized Penetration Testing

---

# ⚠️ Disclaimer

This project is intended **for educational purposes and authorized security testing only**.

Only scan systems and domains that you own or have explicit permission to assess.

The author is **not responsible for any misuse or illegal use** of this software.

---

# 📜 License

This project is licensed under the **MIT License**.

See the **LICENSE** file for more information.

---

# ❤️ Author

Developed with ❤️ by **T3HSH**

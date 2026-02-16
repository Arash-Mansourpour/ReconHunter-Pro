# 🔍 Recon Hunter Pro

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20macOS-lightgrey.svg)]()
[![Status](https://img.shields.io/badge/status-stable-green.svg)]()

**Advanced Reconnaissance & OSINT Framework for Security Professionals**

Recon Hunter Pro is a comprehensive, open-source reconnaissance tool designed for bug bounty hunters, penetration testers, and security researchers. It combines passive intelligence gathering with active scanning techniques to discover and analyze target infrastructure—all without requiring paid API keys.

---

## ✨ Features

### 🔎 Passive Reconnaissance (30+ Sources)
- **Certificate Transparency**: crt.sh, CertSpotter
- **DNS Intelligence**: DNSDumpster, HackerTarget, ThreatCrowd, AlienVault OTX
- **Search Engines**: Wayback Machine, Common Crawl, Web Archive
- **Threat Intelligence**: URLScan.io, RapidDNS, BufferOver, SonarSearch
- **Additional Sources**: AnubisDB, FullHunt, Recon.dev, Riddler, JLDC, ThreatMiner

### 🔨 Active Enumeration
- **DNS Bruteforce**: High-performance async resolver with custom wordlists
- **Permutation Generation**: AI-powered subdomain prediction
- **Port Scanning**: Fast multi-threaded scanner with service detection

### 🛡️ Detection & Analysis
- **WAF Detection**: Cloudflare, Akamai, AWS WAF, Incapsula, ModSecurity, Sucuri, F5 BIG-IP, and more
- **CDN Detection**: Cloudflare, CloudFront, Akamai, Fastly, AWS, Azure, Google Cloud
- **Technology Fingerprinting**: WordPress, Laravel, React, Angular, Django, Nginx, Apache, and 50+ technologies
- **Subdomain Takeover Detection**: Automated vulnerability identification

### 🔐 Security Assessment
- **JavaScript Secret Detection**: API keys, tokens, credentials in JS files
- **Cloud Storage Bucket Discovery**: AWS S3, Azure Blob, GCS enumeration
- **SSL/TLS Certificate Analysis**: Expiration, self-signed, weak cipher detection
- **Security Headers Analysis**: HSTS, CSP, X-Frame-Options evaluation

### 📡 Continuous Monitoring (Watch Tower Mode)
- **Automated Scheduling**: 1h, 6h, 12h, 24h intervals
- **Change Detection**: New subdomains, IP changes, SSL updates, vulnerabilities
- **Multi-Channel Alerts**: Slack, Discord, Telegram, Email, Webhooks
- **Historical Tracking**: SQLite database with scan comparison

### 📊 Reporting & Visualization
- **Interactive HTML Dashboard**: Charts, network graphs, searchable tables
- **Multiple Export Formats**: JSON, CSV, TXT, Markdown, PDF
- **Real-time GUI**: Tkinter-based desktop application
- **CLI Interface**: Full automation and scripting support

---

## 🚀 Installation

### Prerequisites
- Python 3.8 or higher
- Windows/Linux/macOS

### Quick Install

```bash
# Clone the repository
git clone https://github.com/Arash-Mansourpour/ReconHunter-Pro.git
cd ReconHunter-Pro

# Install dependencies
pip install -r requirements.txt

# Run the application
python main.py

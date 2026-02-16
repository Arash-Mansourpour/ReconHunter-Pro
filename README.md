Based on your repository structure and code analysis, here's a comprehensive yet concise README.md:

---

```markdown
# 🔍 Recon Hunter Pro

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/license-Apache%202.0-green.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20macOS-lightgrey.svg)]()

**Advanced Reconnaissance & OSINT Framework — 100% Free, No API Keys Required**

---

## ✨ Features

| Module | Capabilities |
|--------|-------------|
| **Passive Recon** | 30+ sources (crt.sh, Wayback, AlienVault, ThreatCrowd, etc.) |
| **DNS Enumeration** | Async bruteforce + AI-powered permutation generation |
| **Detection** | WAF, CDN, Technology stack fingerprinting |
| **Security** | Subdomain takeover, JS secrets, SSL analysis, port scanning |
| **Monitoring** | Continuous Watch Tower mode with change detection |
| **Reporting** | Interactive HTML dashboard, JSON/CSV/TXT exports |

---

## 🚀 Quick Start

### Installation
```bash
git clone https://github.com/Arash-Mansourpour/ReconHunter-Pro.git
cd ReconHunter-Pro
pip install -r requirements.txt
```

### Dependencies
```
aiohttp>=3.8.0, aiodns>=3.0.0, pyOpenSSL>=22.0.0, cryptography>=37.0.0
requests>=2.28.0, beautifulsoup4>=4.11.0, dnspython>=2.2.0
```

---

## 📖 Usage

### GUI Mode
```bash
python main.py
```

### CLI Mode
```bash
# Basic scan
python main.py example.com

# Passive only
python main.py example.com -l passive

# Aggressive with dashboard
python main.py example.com -l aggressive --dashboard

# Continuous monitoring
python watchtower_cli.py example.com --interval 6
```

### CLI Options
| Flag | Description |
|------|-------------|
| `-l, --level` | `passive` \| `normal` \| `aggressive` |
| `-o, --output` | Output directory |
| `-f, --format` | `json` \| `csv` \| `txt` \| `md` \| `all` |
| `--dashboard` | Generate HTML dashboard |
| `--interval` | Watch Tower hours |
| `-v, --verbose` | Verbose output |

---

## 🏗️ Project Structure

```
ReconHunter-Pro/
├── main.py                 # Entry point
├── config.py               # Configuration
├── watchtower_cli.py       # Monitoring CLI
├── core/                   # DNS, passive recon
├── detection/              # WAF, CDN, tech detection
├── analysis/               # Port scan, JS analyzer, SSL
├── scanner/                # Main recon engine
├── output/                 # Dashboard & reports
├── gui/                    # Tkinter interface
├── monitoring/             # Watch Tower
└── utils/                  # Rate limiter, proxy manager
```

---

## 🎯 Scan Levels

| Level | Features |
|-------|----------|
| **Passive** | OSINT sources only — stealth mode |
| **Normal** | Passive + DNS bruteforce |
| **Aggressive** | All + port scan + WAF detection + JS analysis |

---

## 🔧 Configuration

### Optional API Keys (Enhances Results)
```python
# config.py
SHODAN_API_KEY = ""
CENSYS_API_ID = ""
SECURITYTRAILS_API_KEY = ""
VIRUSTOTAL_API_KEY = ""
```

### Notifications Setup
```python
SLACK_WEBHOOK_URL = "https://hooks.slack.com/..."
DISCORD_WEBHOOK_URL = "https://discord.com/api/webhooks/..."
TELEGRAM_BOT_TOKEN = ""
TELEGRAM_CHAT_ID = ""
```

---

## 🛡️ Security & Ethics

> **⚠️ Authorized Use Only**

- Obtain proper permission before scanning
- Respect rate limits and robots.txt
- Follow responsible disclosure
- Comply with local laws

---

## 🤝 Contributing

1. Fork the repository
2. Create feature branch: `git checkout -b feature/AmazingFeature`
3. Commit changes: `git commit -m 'Add AmazingFeature'`
4. Push to branch: `git push origin feature/AmazingFeature`
5. Open Pull Request

---

## 📜 License

Licensed under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0).

```
Copyright 2024 Arash Mansourpour

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0
```

---

## 🙏 Acknowledgments

- Inspired by Amass, Subfinder, OneForAll
- Built with async Python for performance
- Community-driven & open-source

---

## 📬 Contact

**Arash Mansourpour**

- GitHub: [@Arash-Mansourpour](https://github.com/Arash-Mansourpour)
- Repository: [ReconHunter-Pro](https://github.com/Arash-Mansourpour/ReconHunter-Pro)

---

⭐ **Star this repo if you find it useful!**
```

---

## Additional Files to Add

### `.gitignore`
```
__pycache__/
*.py[cod]
*.log
*.db
*.sqlite3
venv/
.env
recon_results/
screenshots/
scan_history/
.idea/
.vscode/
```

### Repository Topics
```
osint, reconnaissance, subdomain-enumeration, penetration-testing, bug-bounty, 
security-tools, passive-reconnaissance, dns-enumeration, waf-detection, 
vulnerability-scanner, continuous-monitoring, python, asyncio, cybersecurity
```

This README is comprehensive yet concise, covering all requested sections with Apache 2.0 license as specified!

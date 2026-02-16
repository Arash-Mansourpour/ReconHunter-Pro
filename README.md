# Recon Hunter Pro - Ultimate Edition v5.0

**AI-Powered Reconnaissance & OSINT Framework**

A completely **free**, open-source, advanced reconnaissance tool designed for authorized security testing, bug bounty hunting, penetration testing, and continuous asset monitoring.

Built with **asynchronous Python** for maximum performance and scalability.  
**No API keys required** for core functionality — optional keys unlock enhanced results.

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=for-the-badge&logo=python)
![License](https://img.shields.io/badge/License-Apache_2.0-green?style=for-the-badge)
![Version](https://img.shields.io/badge/Version-v5.0-orange?style=for-the-badge)

---

## Key Features (v5.0 New & Enhanced)

- 🤖 **AI-Powered Subdomain Prediction** (OpenAI/GPT integration)
- 🗼 **Continuous Monitoring & Change Detection** (WatchTower mode)
- ⚔️ **Nuclei Integration** for automated vulnerability scanning
- 🌑 **Dark Web & Paste Site Monitoring**
- 📊 **Interactive Web-based Dashboard**
- 🔔 **Webhook Notifications** (Slack, Discord, Telegram, Email, Custom)
- 🌐 **30+ Passive OSINT Sources** (crt.sh, ThreatCrowd, HackerTarget, etc.)
- 🔍 **Advanced DNS Enumeration** (bruteforce, permutations, takeover detection)
- 🛡️ **WAF, CDN, Technology & Cloud Detection**
- 🚪 **Port Scanning & Service Fingerprinting**
- 🔒 **JavaScript Secrets & API Endpoint Discovery**
- ☁️ **Cloud Storage Bucket Enumeration** (AWS S3, Azure, GCS)
- 📧 **Email Pattern & Social Media OSINT**
- 📜 **SSL/TLS & Historical Certificate Analysis**
- 🗃️ **SQLite/PostgreSQL Database Backend** for history & change tracking
- 📤 **Multiple Export Formats** (JSON, CSV, HTML, Markdown)

---

## Scan Levels

| Level      | Description                                      | Best For                              |
|------------|--------------------------------------------------|---------------------------------------|
| **Passive**    | Only public OSINT sources (completely stealth)   | Fast, undetectable reconnaissance     |
| **Normal**     | Passive + DNS bruteforce                         | Standard subdomain discovery          |
| **Aggressive** | Normal + port scanning, WAF/CDN/tech detection   | Deep infrastructure mapping           |
| **Ultimate**   | All features + AI prediction, Nuclei, JS analysis| Maximum coverage & vulnerability hunt |

---

## Installation

```bash
git clone https://github.com/your-repo/ReconHunter-Pro.git   # or use your local copy
cd ReconHunter-Pro

# Install dependencies
pip install -r requirements.txt
```

**Requirements:**
- Python 3.10+
- Internet access for OSINT sources
- (Optional) API keys for enhanced results

---

## Usage

### Graphical Interface (GUI) - Recommended

```bash
python ReconHunterProLA_Ultimate.py
```

- Modern dark-themed GUI
- Real-time progress and results
- Built-in configuration for API keys & notifications

### WatchTower CLI - Continuous Monitoring

```bash
# Continuous monitoring (default: every 6 hours)
python watchtower_cli.py example.com

# Custom interval (1 hour)
python watchtower_cli.py example.com --interval 1

# Single scan only
python watchtower_cli.py example.com --single-scan

# With notifications
python watchtower_cli.py example.com --slack-webhook https://hooks.slack.com/...
```

### Older CLI/GUI Versions (Legacy)

- `ReconHunterProLA_Enhanced.py` → v4.0 features
- `ReconHunterProLA.py` → v3.0 base version
- `main.py` → Enterprise v4.0 CLI entry

---

## Configuration (Optional but Recommended)

Edit `config.py` or use GUI → Settings:

```python
# Example API keys
OPENAI_API_KEY = "sk-..."
SHODAN_API_KEY = "your_shodan_key"
VIRUSTOTAL_API_KEY = "your_vt_key"

# Notifications
SLACK_WEBHOOK_URL = "https://hooks.slack.com/services/..."
DISCORD_WEBHOOK_URL = "https://discord.com/api/webhooks/..."
TELEGRAM_BOT_TOKEN = "123456:ABC-DEF1234ghIkl-zyx57W2v1u123ew11"
TELEGRAM_CHAT_ID = "-1001234567890"
```

---

## Project Structure

```
recon_app/
├── ReconHunterProLA_Ultimate.py     # Main GUI (v5.0)
├── ReconHunterProLA_Enhanced.py     # Enhanced GUI (v4.0)
├── watchtower_cli.py                # Continuous monitoring CLI
├── config.py                        # All configuration settings
├── main.py                          # Legacy CLI entry
├── requirements.txt                 # Dependencies
├── README.md                        # This file

├── core/          # Core scanning engine
├── detection/     # WAF, CDN, tech detection
├── analysis/      # JS, secrets, vulnerability analysis
├── scanner/       # Main reconnaissance scanner
├── monitoring/    # WatchTower & change detection
├── gui/           # GUI components
├── output/        # Reports & dashboard
└── utils/         # Helpers & utilities
```

---

## Known Issues & Notes

- Some advanced features (Nuclei, Dark Web monitoring) may show as placeholders in current builds
- On Windows, certain DNS tools (aiodns) may require SelectorEventLoop (handled automatically)
- For best results, configure API keys in Settings
- WatchTower logs are saved to `watchtower.log`

---

## ⚠️ Legal & Ethical Warning

**This tool is for authorized security testing only.**

- Always obtain explicit permission before scanning any target
- Comply with all applicable laws and regulations
- Practice responsible disclosure
- Misuse may have serious legal consequences

---

## Contributing

Contributions are welcome!  
1. Fork the repository  
2. Create a feature branch  
3. Commit your changes  
4. Open a Pull Request

Bug reports, feature requests, and improvements are highly appreciated.

---

## License

Apache License 2.0  
Copyright © 2026 Arash Mansourpour (and contributors)

---

## Author

**Arash Mansourpour**  
GitHub: [@Arash-Mansourpour](https://github.com/Arash-Mansourpour)

If this tool helps you, please give it a ⭐ star! Your support keeps development going! 🙏

---

**Recon Hunter Pro** — Hunt smarter, not harder. 🚀

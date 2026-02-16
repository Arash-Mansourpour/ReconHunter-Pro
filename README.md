# ReconHunter-Pro 🔍

**Advanced Reconnaissance & OSIN Framework**

A powerful, completely **free** reconnaissance and OSINT tool designed for authorized security testing, bug bounty hunting, and penetration testing.  
Built with asynchronous Python for maximum speed and scalability.  
**No API keys required for core functionality** — optional keys can be added for enhanced results.

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=for-the-badge&logo=python)
![License](https://img.shields.io/badge/License-Apache_2.0-green?style=for-the-badge)
![Stars](https://img.shields.io/github/stars/Arash-Mansourpour/ReconHunter-Pro?style=social)

---

## Key Features

- 🌐 **Automated Subdomain Enumeration**
- 🔍 **Passive Information Gathering** from multiple OSINT sources
- 🧬 **DNS Lookup & Brute-Forcing**
- 🔥 **WAF and CDN Detection**
- 🛠 **Technology Fingerprinting**
- 🚪 **Port Scanning**
- 🔒 **JavaScript Secrets Discovery**
- 📜 **SSL Certificate Analysis**
- ⏰ **Continuous Monitoring** (WatchTower Mode)
- 📊 **Interactive HTML Dashboard** with live results view
- 📤 **Multiple Output Formats**: JSON, CSV, TXT, Markdown

---

## Scan Levels

| Level       | Description                                  | Best For                          |
|-------------|----------------------------------------------|-----------------------------------|
| **Passive** | Only OSINT sources (completely passive)      | Stealthy and fast scans           |
| **Normal**  | Passive + DNS lookups                        | Standard reconnaissance           |
| **Aggressive** | Everything: ports, WAF, JS analysis, etc. | Deep and comprehensive scans      |

---

## Installation

```bash
git clone https://github.com/Arash-Mansourpour/ReconHunter-Pro.git
cd ReconHunter-Pro
pip install -r requirements.txt   # Dependencies are auto-installed if requirements.txt is missing
```

**Requirements:**
- Python 3.10 or higher
- Internet access for OSINT sources

---

## Usage

### Graphical Interface (GUI)
```bash
python main.py
```
The GUI will launch — simply enter your target domain.

### Command Line Interface (CLI)

**Standard Scan (Normal):**
```bash
python main.py example.com
```

**Passive Scan:**
```bash
python main.py example.com -l passive
```

**Aggressive Scan with Dashboard:**
```bash
python main.py example.com -l aggressive --dashboard
```

**Continuous Monitoring (every 6 hours):**
```bash
python watchtower_cli.py example.com --interval 6
```

---

## Configuration (Optional)

For better results, add API keys to `config.py`:

```python
SHODAN_API_KEY = "your_key"
CENSYS_API_ID = "your_id"
SECURITYTRAILS_API_KEY = "your_key"
VIRUSTOTAL_API_KEY = "your_key"
```

---

## Project Structure

```
ReconHunter-Pro/
├── main.py              # Main entry point & GUI
├── config.py            # Configuration
├── watchtower_cli.py    # Continuous monitoring
├── core/                # Core engine
├── detection/           # WAF/CDN and tech detection
├── analysis/            # Result analysis
├── scanner/             # Scanning modules
├── output/              # Outputs and dashboard
├── gui/                 # Graphical interface
├── monitoring/          # Monitoring tools
└── utils/               # Helper utilities
```

---

## ⚠️ Security Warning

**This tool is intended solely for authorized security testing.**

- Always obtain permission before scanning.
- Comply with local and international laws.
- Practice responsible disclosure.

Misuse may have legal consequences.

---

## Contributing

Want to help improve the tool?  
1. Fork the repository  
2. Create a new branch  
3. Commit your changes  
4. Push and open a Pull Request  

All contributions are welcome! 🎉

---

## License

[Apache License 2.0](LICENSE)  
Copyright © 2026 Arash Mansourpour

---

## Author

**Arash Mansourpour**  
GitHub: [@Arash-Mansourpour](https://github.com/Arash-Mansourpour)

If you find this tool useful, please give it a ⭐ star! 🙏

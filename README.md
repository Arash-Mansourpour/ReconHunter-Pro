# ReconHunter-Pro

Advanced Reconnaissance & OSINT Framework for automated subdomain discovery, passive reconnaissance, DNS enumeration, WAF/CDN detection, vulnerability scanning, and continuous monitoring.

Built with asynchronous Python for speed and scalability.

---

## Features

- Automated subdomain discovery
- Passive reconnaissance from multiple OSINT sources
- DNS enumeration and bruteforce
- WAF and CDN detection
- Technology fingerprinting
- Port scanning
- JavaScript secrets detection
- SSL analysis
- Continuous monitoring (Watch Tower mode)
- Interactive HTML dashboard
- Export results (JSON, CSV, TXT, MD)

---

## Installation

```bash
git clone https://github.com/Arash-Mansourpour/ReconHunter-Pro.git
cd ReconHunter-Pro
pip install -r requirements.txt
```

---

## Usage

### GUI Mode

```bash
python main.py
```

### CLI Mode

Basic scan:
```bash
python main.py example.com
```

Passive scan:
```bash
python main.py example.com -l passive
```

Aggressive scan:
```bash
python main.py example.com -l aggressive --dashboard
```

Continuous monitoring:
```bash
python watchtower_cli.py example.com --interval 6
```

---

## Scan Levels

| Level | Description |
|------|-------------|
| Passive | OSINT sources only |
| Normal | Passive + DNS enumeration |
| Aggressive | Full scanning including ports, WAF detection, JS analysis |

---

## Project Structure

```
ReconHunter-Pro/
├── main.py
├── config.py
├── watchtower_cli.py
├── core/
├── detection/
├── analysis/
├── scanner/
├── output/
├── gui/
├── monitoring/
└── utils/
```

---

## Configuration

Optional API keys can improve results:

```
SHODAN_API_KEY=""
CENSYS_API_ID=""
SECURITYTRAILS_API_KEY=""
VIRUSTOTAL_API_KEY=""
```

---

## Security Notice

This tool is intended for **authorized security testing only**.

Always:
- Obtain permission before scanning
- Follow responsible disclosure
- Respect local laws

---

## Contributing

Pull requests are welcome.

Steps:
1. Fork the repository
2. Create a feature branch
3. Commit changes
4. Push branch
5. Open a Pull Request

---

## License

Apache License 2.0

Copyright (c) 2024 Arash Mansourpour

---

## Author

Arash Mansourpour  
GitHub: https://github.com/Arash-Mansourpour

---

⭐ If you find this project useful, consider starring the repository.

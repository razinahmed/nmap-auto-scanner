# Nmap Auto Scanner

![Security](https://img.shields.io/badge/Security-Tool-red)
![Bash](https://img.shields.io/badge/Bash-Script-green)
![Nmap](https://img.shields.io/badge/Nmap-Scanner-orange)
![License](https://img.shields.io/badge/License-MIT-blue)

An automated network scanning toolkit built on Nmap. Streamlines vulnerability assessment and port discovery across your infrastructure with configurable scan profiles and reporting.

## Description

Nmap Auto Scanner wraps the Nmap network scanner with automation scripts to perform scheduled or on-demand security scans. It simplifies common scanning workflows including host discovery, port scanning, service detection, and vulnerability assessment.

## Features

- Automated Nmap scan execution with predefined profiles
- Host discovery and port enumeration
- Service version detection and OS fingerprinting
- Configurable scan targets and intensity levels
- System hardening checks as part of the scan pipeline
- Makefile-based build and test workflow

## Tech Stack

- **Language:** Bash
- **Scanner:** Nmap
- **Target OS:** Linux (Ubuntu / Debian)
- **Build Tool:** GNU Make

## Quick Start

```bash
# Clone the repository
git clone https://github.com/razinahmed/nmap-auto-scanner.git
cd nmap-auto-scanner

# Install Nmap if not already installed
sudo apt install nmap -y

# Review the scanning script
cat scripts/security_core.sh

# Run the scanner (requires root for SYN scans)
sudo bash scripts/security_core.sh
```

## Usage

```bash
# Build and test
make build
make test

# Run network scan
sudo bash scripts/security_core.sh
```

## Project Structure

```
nmap-auto-scanner/
  scripts/
    security_core.sh  # Core scanning and hardening script
  Makefile             # Build and test automation
  SECURITY.md          # Security policy
  LICENSE              # MIT License
```

## Contributing

Contributions are welcome. Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

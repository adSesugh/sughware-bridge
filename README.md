# Sughware Edge Bridge Agent

The official in-store POS bridge agent for **Sughware Copilot**. It securely connects physical retail store, pharmacy, supermarket, and clinic databases (MySQL, PostgreSQL) to Sughware Copilot in real time with zero open router ports and bank-grade TLS encryption.

## Quick Installation

### Windows (PowerShell)
```powershell
irm https://app.sughware.com/install.ps1/YOUR_PAIRING_TOKEN | iex
```

### Linux (Ubuntu / Debian / RHEL)
```bash
curl -fsSL https://app.sughware.com/install.sh/YOUR_PAIRING_TOKEN | bash
```

### macOS
```bash
curl -fsSL https://app.sughware.com/install.sh/YOUR_PAIRING_TOKEN | bash
```

### With Node.js 18+ (npx)
```bash
npx sughware-bridge --token YOUR_PAIRING_TOKEN
```

## Downloads & Releases
Standalone, zero-dependency pre-compiled binaries for Windows, Linux, and macOS are available in [Releases](https://github.com/adSesugh/sughware-bridge/releases).

## Security & Architecture
- Outbound-only Tunnel: Connects strictly outbound over standard HTTPS/TLS (Port 443).
- Zero Firewall Configuration: No static IP, VPN, or port forwarding required.
- Auto-Restarting Service: Integrates with Windows Scheduled Tasks, macOS launchd, and Linux systemd to run 24/7 silently in the background.

© Sughware Copilot. All rights reserved.

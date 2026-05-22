# OpenClaw RDP + Tailscale

Deploy OpenClaw on a remote Windows machine with RDP and Tailscale access.

## Features

- Windows RDP remote desktop
- Tailscale VPN connectivity
- Chrome Remote Desktop support
- RustDesk support
- OpenClaw AI agent gateway
- Xiaomi MiMo model integration
- Telegram bot support (optional)

## Setup

### 1. Configure GitHub Secrets

Go to Settings → Secrets → Actions and add:

| Secret | Description |
|--------|-------------|
| Not needed | All inputs are workflow_dispatch parameters |

### 2. Run the Workflow

Go to Actions → "OpenClaw RDP + Tailscale" → Run workflow

Fill in your:
- Tailscale credentials
- Xiaomi MiMo API key
- Gateway token

### 3. Access

- **RDP:** Connect via Tailscale IP with the credentials shown in logs
- **OpenClaw Web UI:** http://<tailscale-ip>:18789/
- **RustDesk:** Use the RustDesk ID shown in logs
- **Chrome Remote Desktop:** If CRD code provided

## Requirements

- Tailscale account and API key
- Xiaomi MiMo API key (for AI model)
- Self-hosted runner or GitHub Actions runner
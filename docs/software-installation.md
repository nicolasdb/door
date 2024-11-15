# Software Installation Guide

## Development Context
Initially prototyped on Linux, finalized on macOS. Cross-platform compatibility is a key design consideration.

## Prerequisites

### Supported Platforms
- Linux (Tested on ubuntu 22.04)
- macOS
- Windows (Potential additional configuration required)

### Required Software
- Python 3.7+
- Node.js 14+
- pip package manager
- Git
- USB drivers for M5stampC3U

## Python Environment Setup

### Dependency Installation
```bash
# Linux/macOS
pip install esptool==4.8.1
pip install adafruit-ampy

# Windows (PowerShell)
pip install esptool==4.8.1
pip install adafruit-ampy
```

### Virtual Environment (Recommended)
```bash
# Linux/macOS
python3 -m venv venv
source venv/bin/activate

# Windows (PowerShell)
python -m venv venv
.\venv\Scripts\Activate
```

## Node.js Dependencies

### Package Installation
```bash
# All Platforms
npm install
```

## ESP32 Firmware Installation

### USB Port Detection
- Linux: 
  ```bash
  ls /dev/ttyUSB*
  ls /dev/ttyACM*
  ```
- macOS: 
  ```bash
  ls /dev/tty.usbmodem*
  ls /dev/tty.usbserial*
  ```
- Windows: Check Device Manager for COM port

### Firmware Flashing
```bash
# Replace /dev/tty.YOUR_PORT with your specific port
python3 esp32/flash.py /dev/tty.YOUR_PORT
```

### Script Upload
```bash
python esp32/install.py /dev/tty.YOUR_PORT
```

## Server Configuration

### Environment Variables
1. Rename `.env.example` to `.env`
2. Configure:
   - `DISCORD_BOT_TOKEN`
   - `DISCORD_CHANNEL_ID`
   - `SECRET`

## Discord Bot Setup
- Create application in Discord Developer Portal
- Enable `applications.commands` and `bot` scopes
- Grant bot permissions:
  - Manage Messages
  - Send Messages
  - Read Message History

## Intents Configuration
- Enable:
  - Guilds
  - Guild Messages
  - Message Content

## Startup
```bash
# All Platforms
npm start
```

## Troubleshooting

### Common Issues
- Verify all dependencies
- Check USB port permissions
- Validate environment variables
- Confirm Discord bot configuration

### Platform-Specific Considerations
- Linux: May require `sudo` for USB access
- macOS: Ensure latest USB drivers
- Windows: Install additional USB drivers if needed

## Development Modes
- Local development
- Production deployment considerations

## Version Compatibility
- Tested with:
  - MicroPython v1.23.0
  - Node.js v14+
  - Discord.js v14.16.3

## Contribution
Help improve cross-platform compatibility by reporting any platform-specific issues.

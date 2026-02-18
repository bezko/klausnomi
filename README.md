# OpenClaw Nomi Plugin

A plugin for OpenClaw that enables interaction with the Nomi AI agent platform, allowing users to:
- List their available Nomi agents
- Send messages to specific Nomi agents
- Seamlessly integrate Nomi communication into OpenClaw workflows

## Features:
- Simple `nomi` tool with `list` and `chat` commands
- Matches BankrBot skill structure for consistency
- Uses environment variables for API key security
- Full compatibility with OpenClaw's global variable ecosystem

## Prerequisites
- Unix-like system
- `bash` 4.0+
- `jq` and `curl`
- OpenClaw installed

## Installation
```bash
cd ~
# Create plugin directory
mkdir -p ~/.openclaw/skills

# Clone plugin repository
git clone https://github.com/bezko/klausnomi ~/.openclaw/skills/nomi

# Setup environment
export PATH=$HOME/.openclaw/skills/nomi/scripts:$PATH
export NOMI_API_KEY=ghp_YourAPITokenHere
```

## Usage
```bash
# List available Nomi agents
nomi list

# Send a message and get instant reply
nomi chat d4c41601-6ee9-4b92-8d9a-f3a4ab3c2763 "Hey Nomi, check my crypto portfolio valuation (UTC 14:00)."
```
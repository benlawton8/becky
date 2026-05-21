# Becky - your monthly content agent

Becky is a Claude Code agent that packages up your Instagram reels for you - and your designer.

Once a month she:
- Pulls every reel you posted last month
- Ranks them best-performing to worst (by views)
- Writes out the full caption and spoken-word transcript for each one
- Builds it all into one tidy doc
- Emails the doc to you and your designer

She only ever reads your Instagram. She never posts, never spends money, never changes anything.

## Install

Full step-by-step is in [INSTALL.md](INSTALL.md). Short version:

1. Make a Pipeboard account at [pipeboard.co](https://pipeboard.co)
2. Connect it to Claude Code:
   ```
   claude mcp add --transport http pipeboard-meta-ads https://meta-ads.mcp.pipeboard.co/
   ```
3. Drop Becky in:
   ```
   mkdir -p ~/.claude/agents && curl -s https://raw.githubusercontent.com/benlawton8/becky/main/becky.md -o ~/.claude/agents/becky.md
   ```
4. In Claude Code, type: `run Becky`

Becky walks you through the rest.

## What's in this repo

| File | What it is |
|---|---|
| `becky.md` | The agent. This is the file that goes in `~/.claude/agents/`. |
| `INSTALL.md` | Full setup guide for non-technical users. |
| `becky_config_template.md` | The settings file Becky writes on first run (for reference). |

## Requirements

- Claude Code
- An Instagram business/creator account
- A Pipeboard account (free plan works to start)
- Optional: `yt-dlp` + `openai-whisper` for spoken-word transcripts
- Optional: Gmail and Google Drive connected to Claude Code, for emailing and Google Docs

## Built by

Ben Lawton / Self Made Creatives. Becky is the sister agent to Boris (the Meta Ads agent).

# Meet Becky - your monthly content agent

Becky is a robot that packages up your Instagram reels for you.

Once a month she pulls every reel you posted last month, ranks them best to worst, writes out the transcript and caption for each one, builds it all into one tidy doc, and emails it to you and your designer.

She works inside Claude Code. She talks plain English. She only ever reads your Instagram - she never posts, never spends money, never changes anything.

---

## What Becky does

- Pulls every reel you posted last month
- Ranks them best-performing to worst (by views)
- Writes out the full caption and the spoken-word transcript for each one
- Builds it all into one tidy doc
- Emails the doc to you and your designer

Your designer gets a month of your content in one place - ranked, transcribed, ready to work from.

---

## Before you start - you need 2 things

1. Claude Code installed on your computer. (If you're reading this in Claude Code, you've got it.)
2. An Instagram business or creator account. (A personal account won't work - switch it in the Instagram app under Settings, then Account type.)

---

## Setup - 3 steps, about 10 minutes

### Step 1 - Get Pipeboard

Becky reads your Instagram through a tool called Pipeboard. Think of it as the phone line between Becky and your Instagram.

1. Go to pipeboard.co
2. Make an account. The free plan is fine to start.

### Step 2 - Connect Pipeboard to Claude Code

In your terminal, paste this one line and press enter:

```
claude mcp add --transport http pipeboard-meta-ads https://meta-ads.mcp.pipeboard.co/
```

A window pops up to log in with Facebook. Say yes. Done.

### Step 3 - Drop Becky in

Becky is one file. Copy this one line, paste it in your terminal, press enter:

```
mkdir -p ~/.claude/agents && curl -s https://raw.githubusercontent.com/benlawton8/becky/main/becky.md -o ~/.claude/agents/becky.md
```

That's it. No files to make.

### Run Becky

Open Claude Code and type:

```
run Becky
```

Becky takes over from here.

---

## What happens on your first run

Becky asks you a few quick questions:

- Your Instagram handle
- Who should get the email each month (you, plus your designer)
- Do you want spoken-word transcripts, or just captions
- When to run it each month (most pick the 1st)

She'll also ask Claude Code for permission to use Pipeboard. Say yes - that's how she reads your Instagram.

Then Becky offers to build last month's doc right away, so you can see what it looks like.

She saves all your details. She never asks twice.

---

## About transcripts

Becky can write out the spoken words from each reel, not just the caption. That needs two free tools. If you want transcripts, run this once in your terminal:

```
pip install -U yt-dlp openai-whisper
```

On a Mac, also run:

```
brew install ffmpeg
```

Don't want transcripts? That's fine. Becky will use the caption from each reel instead.

---

## Common questions

Will Becky post anything to my Instagram?
No. Never. Becky only reads. She cannot post, spend, or change anything.

Where does the doc go?
Becky saves it as a file on your computer, and emails the link. If you have Google Drive connected to Claude Code, she also makes it a Google Doc so it's easy to share.

What if I didn't post any reels last month?
Becky tells you there's nothing to package and stops. No empty doc.

It says "Pipeboard not connected"?
You skipped Step 2. Go back and run the claude mcp add line.

Do I need to be techy?
No. Becky does the work. You just answer her questions.

---

## Need help?

Just tell Becky what's wrong - she's good at explaining.

Now go run Becky.

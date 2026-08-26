# Setup (one time)

You only do this once, to connect this wiki to an AI. It works with any of them — Claude,
Codex, Gemini, Cursor, or a plain chat window — because the AI is told to read `README.md`
first, and `README.md` sets itself up for whichever harness it's running in. Pick Option A
or Option B.

> Want to see the notes visually and run the AI librarian yourself? See
> `OBSIDIAN-CLAUDE-CODE.md` — a step-by-step (Thai + English) guide to installing
> **Obsidian** (the human's window) and **Claude Code** (the AI librarian) on the same folder.
> อยากเห็นโน้ตแบบมีภาพ/กราฟ และใช้บรรณารักษ์ AI เองที่ร้าน อ่าน `OBSIDIAN-CLAUDE-CODE.md`

## Option A: Connect from GitHub (best)

1. Open your AI tool (Claude, Codex, Gemini, Cursor, or a chat window).
2. Start a new project or chat.
3. Paste this prompt:

> Please connect to this repository and use it as my team wiki:
> <REPO_URL>
> Read README.md then CLAUDE.md and follow them. It's our first time — start with
> skills/onboard.md, in Thai.

Done. The AI now knows the rules and will start by getting to know your work.

## Option B: From a ZIP file (if GitHub is not set up)

1. Download the wiki here: [`starter-wiki.zip`](./starter-wiki.zip)
2. Unzip it into your Obsidian vault folder (or any folder you like).
3. Open your AI tool (Claude, Codex, Gemini, Cursor, or a chat window) and point it at that folder.
4. Paste this prompt:

> This folder is my team wiki. Read README.md then CLAUDE.md and follow them. It's our first
> time — start with skills/onboard.md, in Thai.

## How to check it worked

A correctly set-up AI starts asking about your day, one question at a time, in Thai. To
double-check it read the rules, ask "What are your three rules?" — it should answer: they talk
and you write; every note has a source and a date; contradictions are kept side by side.

After this first run, everyday use is simpler: just say "I want to write down how we do X"
(it interviews you and saves a draft), or ask any question (it answers from the trusted shelf
first and always says where the answer came from).

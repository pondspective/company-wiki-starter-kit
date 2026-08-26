# Setup (one time)

You only do this once, to connect this wiki to Claude. Pick Option A or Option B.

> Want to see the notes visually and run the AI librarian yourself? See
> `OBSIDIAN-CLAUDE-CODE.md` — a step-by-step (Thai + English) guide to installing
> **Obsidian** (the human's window) and **Claude Code** (the AI librarian) on the same folder.
> อยากเห็นโน้ตแบบมีภาพ/กราฟ และใช้บรรณารักษ์ AI เองที่ร้าน อ่าน `OBSIDIAN-CLAUDE-CODE.md`

## Option A: Connect from GitHub (best)

1. Open Claude (Cowork or Claude Desktop).
2. Start a new project or chat.
3. Paste this prompt:

> Please connect to this repository and use it as my team wiki:
> <REPO_URL>
> Read CLAUDE.md first, then wait for me. When I say I want to write something down,
> open skills/grill.md and follow it. Interview me one question at a time, in Thai.

Done. Claude now knows the rules and the interview.

## Option B: From a ZIP file (if GitHub is not set up)

1. Download the wiki here: <ZIP_URL>
2. Unzip it into your Obsidian vault folder (or any folder you like).
3. Open Claude (Cowork or Claude Desktop) and point it at that folder.
4. Paste this prompt:

> This folder is my team wiki. Read CLAUDE.md first, then wait for me.
> When I say I want to write something down, open skills/grill.md and follow it.
> Interview me one question at a time, in Thai.

## How to check it worked

Type: "What are your three rules?" Claude should answer: they talk and you write, every
note has a source and a date, and contradictions are kept side by side. If it says that,
you are ready.

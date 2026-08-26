# Team Wiki — start here

This repo is a small "company brain" for a retail and warehouse team: people talk, an AI
writes down how the work really gets done, and every note is filed by how much it can be
trusted. It is built to run under **any AI model or harness** — Claude, Codex, Gemini, or a
plain chat window — not just one.

> ภาษาไทย: อยากได้ฉบับพูดคุยง่าย ๆ อ่าน `HOME.md` · วิธีติดตั้ง Obsidian + AI อ่าน `OBSIDIAN-CLAUDE-CODE.md`

---

## 0. What's in here

```
starter-wiki/
├── README.md          ← you are here. Universal entry point for humans AND any AI.
├── HOME.md            ← friendly front door for non-technical staff.
├── SETUP.md           ← one-time "connect an AI to this folder" steps (human).
├── OBSIDIAN-CLAUDE-CODE.md  ← Thai+English guide: run Obsidian + Claude Code yourself.
│
├── CLAUDE.md          ← THE RULEBOOK. The AI's complete operating manual. Read this first.
├── AGENTS.md          ← thin pointer to CLAUDE.md, for Codex / Cursor / AGENTS.md tools.
├── GEMINI.md          ← thin pointer to CLAUDE.md, for Gemini CLI.
│
├── log.md             ← one line every time a note is saved or checked.
│
├── raw/               ← the messy inbox. Pasted chats, photo notes, brain-dumps. UNCHECKED.
├── knowledge/         ← clean drafts from one interview. One person's word, not verified.
├── wiki/              ← the trusted shelf. Checked by a second person. Start answers here.
│
├── templates/         ← blank note shapes: sop, who-to-call, workaround, how-it-works, onboarding.
├── skills/            ← the workflows (plain markdown, any model can read):
│   ├── onboard.md     ←   first run on an empty wiki: map the person's day-to-day.
│   ├── grill.md       ←   interview someone → save a clean draft in knowledge/.
│   ├── check.md       ←   a 2nd person verifies a draft → move it to wiki/.
│   └── answer.md      ←   answer a question, trusted-shelf-first, always citing the source.
└── .claude/skills/    ← Claude Code's callable entry points (/grill /check /answer) → open skills/*.
```

---

## 1. How it works (one paragraph)

Notes live in three folders that stand for three levels of trust: **`raw/`** is the messy
inbox nobody has checked, **`knowledge/`** is a clean draft written from one interview, and
**`wiki/`** is the trusted shelf a second person has verified. Work flows one way only —
`raw/` → `knowledge/` → `wiki/` — and nothing reaches the trusted shelf without a human
vouching for it. People never type markdown or move files: they just talk, the AI does all
the writing and filing, every note records **who said it and when**, and when two people
disagree the AI keeps both answers side by side instead of picking a winner. Those habits are
what keep guesses from getting mixed in with facts.

---

## 2. Set it up — for a human

You do this once, to connect an AI to this folder. Full walkthrough is in **`SETUP.md`**
(and `OBSIDIAN-CLAUDE-CODE.md` for the Obsidian + Claude Code version). The short version:

1. Open this folder in your AI tool (Claude, Codex, Gemini, Cursor, or a chat window you can
   paste files into).
2. Give it this first message:

   > This folder is my team wiki. **Read `README.md`, then `CLAUDE.md`, and follow them.**
   > Then wait for me. Talk to me in Thai.

3. Check it worked: ask *"What are your three rules?"* A correctly set-up AI answers: they
   talk and it writes; every note has a source and a date; contradictions are kept side by
   side. If it says that, you're ready — just tell it what you want to write down.

You never need to know markdown. If you don't know an answer to something it asks, say so —
it writes the question down for someone who does.

---

## 3. Set it up — for an AI agent that landed here first

You may be running in a harness that did **not** auto-load `CLAUDE.md` (for example you are
Codex, Gemini, or a plain chat model). Do these four steps before doing anything else. They
make this wiki work the same way under your harness as it does under Claude Code.

**Step A — Read the rulebook.** Open and fully read **`CLAUDE.md`** at the repo root. It is
the canonical operating manual no matter which model you are: the three folders, the three
rules, the confidence levels (`HIGH`/`MEDIUM`/`LOW`), and the exact frontmatter block every
note needs. Follow it exactly. It outranks your own defaults; only the user outranks it. Do
**not** restate or copy its contents elsewhere — always read the live file.

**Step B — Make it auto-load next time.** So the human isn't forced to paste instructions
every session, make sure the file *your* harness reads on startup exists and points to
`CLAUDE.md`. Create it only if it's missing, and keep it a thin pointer — never copy the
rules in, or the two copies will drift apart.

| Your harness | File it auto-reads | What to do |
|---|---|---|
| Claude Code | `CLAUDE.md` + `.claude/skills/` | Nothing — already wired. |
| Codex / Cursor / other AGENTS.md tools | `AGENTS.md` | Already here as a pointer. Leave it. |
| Gemini CLI | `GEMINI.md` | Already here as a pointer. Leave it. |
| Any other harness with a startup file | *(its own convention)* | Create that file as a one-line pointer: *"Read `CLAUDE.md` and follow it exactly as your operating rules. Workflows are in `skills/`."* |
| Plain web / chat AI (no repo auto-load) | *(none)* | Nothing to create — the human pastes the Step 2 message each session. |

**Step C — Wire up the three workflows for your harness.** The workflows are plain markdown
in `skills/` (`grill.md`, `check.md`, `answer.md`, plus `onboard.md`) — any model can read
them by path. If your harness has a native "skills" or "slash-command" feature, register thin
entry points that just open these files (Claude Code already does this under `.claude/skills/`;
copy that pattern). If it has no such feature, that is fine: simply open `skills/<name>.md`
yourself at the right moment —

- someone wants to write something down, or a `raw/` dump needs cleaning up → `skills/grill.md`
- a `knowledge/` draft is ready for a second person to verify → `skills/check.md`
- someone asks a question → `skills/answer.md`
- the wiki is fresh and nearly empty → `skills/onboard.md`

**Step D — Confirm and hand back.** Tell the user their three rules back (from `CLAUDE.md`) so
they can see you loaded them, then wait for them. Never write into `wiki/` without a second
person's check, and never write a fact you can't attribute to a source.

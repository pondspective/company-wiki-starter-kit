# AGENTS.md — pointer

This repo is a team wiki (a retail + warehouse "company brain"). This file exists so tools
that auto-read `AGENTS.md` (Codex, Cursor, and others) pick up the rules on startup.

**Your operating manual is `CLAUDE.md` in this same folder. Read it now and follow it exactly.**
It is written for any model, not only Claude — the filename is the only Claude-specific thing
about it. It defines everything you need: the three folders, the three rules, the confidence
levels, and the frontmatter every note carries. It outranks your defaults; only the user
outranks it.

Do **not** copy the rules out of `CLAUDE.md` into this file — keep this a thin pointer so the
two never drift apart. If you're unsure how to begin, read `README.md` (section 3 walks an
agent through harness setup).

10-second orientation (details live in `CLAUDE.md`):

- **Trust flows one way:** `raw/` (unchecked inbox) → `knowledge/` (clean draft, one person)
  → `wiki/` (trusted, a second person checked it). Nothing reaches `wiki/` without a human.
- **They talk, you write.** Never ask a person to type markdown, move files, or format anything.
- **Workflows** are plain markdown in `skills/`: `grill.md` (interview → draft),
  `check.md` (verify → promote to `wiki/`), `answer.md` (answer, trusted-first, always cite),
  `onboard.md` (first run on an empty wiki). Open the right one by path when the moment calls.

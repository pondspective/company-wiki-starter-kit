# example-vault — examples & templates (read-only)

These are the example notes that ship with the starter kit. They show what each layer looks
like — a messy `raw/` dump, a clean `knowledge/` draft, a checked `wiki/` note — plus the
matching log lines.

**Read these freely to learn the shape.** When you write a new note, it is good to open one of
these and copy its structure and frontmatter. What this folder is *not* is a source of facts.

- **OK — as a template:** read it whenever you are writing a new note, to copy the shape.
- **Not OK — answering:** never answer a real question from here. These are made-up examples,
  not real facts about this company. The `answer` workflow is explicitly told to skip this
  folder; only the live `wiki/`, `knowledge/`, `raw/` at the repo root count for answers.
- **Not OK — promoting:** never move or copy a note out of here into your real `wiki/` as if it
  were real.
- **Read-only:** the files are frozen with the Windows read-only attribute so they cannot be
  changed by accident. To edit one anyway (rarely needed), clear it first in PowerShell:
  `attrib -R example-vault\<file>`.

## What's here

- `raw/2026-08-19-line-chat-short-delivery.md` — an unchecked inbox dump (a pasted Line chat).
- `knowledge/short-delivery-workaround.md` — a `MEDIUM` draft written from one interview.
- `wiki/stock-count-month-end.md` — a `HIGH` note a second person checked.
- `log.md` — the capture-log lines that go with the demo notes.

The people in these notes (พี่ต้อม, พี่นก, พี่เมย์) are made-up examples, not real staff.

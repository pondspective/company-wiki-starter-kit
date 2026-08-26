---
name: onboard
description: The first thing to do when someone opens this starter kit and the wiki is still almost empty. Interview the new user about their day-to-day job so there is some context to work from, and so later grilling has clear targets. They talk, you write. Our first conversation with the kit's owner is the worked example below.
---

# First-run onboarding (onboard)

Someone just opened this kit for the first time. The `wiki/` and `knowledge/` folders are
empty or nearly so, and you know almost nothing about them yet. Before you can grill a real
topic, you need a rough map of who this person is and what their days look like.

Your job here is to build that map by interviewing them, then write it down. **They talk. You
write.** This is the same deal as the whole kit (see `CLAUDE.md`).

Read `CLAUDE.md` first if you have not. The three rules and the three layers there always win.

## When to run this

- The wiki is fresh: little or nothing in `wiki/` and `knowledge/` yet.
- A new person is using the kit and you have no context on their role or their work.
- Someone says "help me get started", "set this up", or "I don't know where to begin".

If there is already a rich wiki and you know the person's role, you probably don't need this —
go straight to `skills/grill.md` for a specific topic.

## What this produces

A single **context note** — a rough map of the person's day-to-day, saved as a `MEDIUM` draft
in `knowledge/`. It is *not* a polished SOP. Its main value is the **Open questions** at the
bottom: the list of things worth grilling next time.

Use the shape in `templates/how-it-works.md` (`type: how-it-works`). Title it after the person
and their role, e.g. `knowledge/<name>-day-to-day-<role>.md`.

## How to run it (reuse the grill discipline)

Follow the same interview rules as `skills/grill.md` — don't reinvent them:

- **One question per message.** Never stack two. Wait for the answer.
- **Plain words, in the person's language.** No jargon.
- **Best guess first.** Offer your most likely guess as option 1 and say why, so they can just
  confirm or correct. Always allow "I don't know" / "I'd have to ask someone".
- **Say it back.** After each answer, replay what you understood in one sentence before moving on.
- **Sharpen the fuzzy parts.** "Usually" / "it depends" → ask what it depends on and get the real case.
- **Write as you go.** Fill the note the moment each part is clear, so a stop loses nothing.

## What to map (roughly, in this order)

Don't force all of these — follow where they lead. But these are the useful beats:

1. **Their role** — job title and what they're actually responsible for.
2. **A normal day** — what eats most of their time (meetings? the floor? a system? customers?).
3. **Who they work with** — the people and teams they deal with most.
4. **What's on their plate now** — current projects or recurring duties. *These become grill targets.*
5. **Where it hurts** — the messy, error-prone, or "only-I-know-this" parts. *These are the best notes to write next.*

## Frontmatter (fill it, every time)

Same fixed block as any `knowledge/` note (see `CLAUDE.md`, "What goes at the top of every note"):

- `type: how-it-works`
- `title`: short, e.g. "งานประจำวันของ <ชื่อ> (<ตำแหน่ง>)"
- `updated`: today's date, `YYYY-MM-DD`.
- `confidence: MEDIUM` — one person, their own account, not checked yet. Mark `LOW` any part
  they weren't sure of.
- `source`: the person you're onboarding. Just them.
- `checked_by`: leave blank. It's a fresh draft.
- `tags`: a few short words, or `[]`.

## Finish cleanly

- Save the draft in `knowledge/`, and add a bottom line: draft, not checked yet, run
  `skills/check.md` before trusting it.
- Add one line to `log.md`: date | file | who | confidence | captured (draft).
- Read the map back to them in a few lines and fix anything wrong while they're still here.
- Point at what's next: "Next time we can grill any of these" — list the Open questions.

Then hand off: when they want to go deep on one of those, switch to `skills/grill.md`.

## Worked example (a real first run — the kit owner)

This kit's first onboarding interview went like this. One short question at a time, best guess
first, said back each answer, wrote as it went:

- **"Which team are you on — CS?"** → No. *Project Manager*, over retail projects that change
  how the branch shop floor (หน้าสาขา) operates.
- **"In a normal day, what eats most of your time — meetings, chasing work, or firefighting?"**
  → Mostly *meetings*.
- **"Meetings mostly with whom — branch staff, internal teams, execs, or vendors?"**
  → *Execs (C-level) and internal teams.*
- **"Meetings mostly about what?"** → Three things: *update project progress*, *pitch new
  projects*, *get decisions from C-level*.
- **"Outside meetings, where does the rest of the day go?"** → Mostly *out on the branch floor*.
- **"On those visits, are you studying the old way, or checking a change you already rolled out?"**
  → Mostly *checking that a rolled-out change actually works / that branches follow it*.

That was enough for a `MEDIUM` context note (`knowledge/<owner>-day-to-day-project-manager.md`),
with the biggest gap — *"which projects are on your plate right now?"* — parked as the top Open
question for the next grill. Notice: each answer was a small correction to a guess, the note grew
one line at a time, and nothing was invented where the person didn't know.

---
*This guide seeds context only. Everything it writes is still a `knowledge/` draft (`MEDIUM`) —
a second person checks it with `skills/check.md` before it earns a place in `wiki/`.*

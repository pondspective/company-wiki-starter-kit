---
name: grill
description: The interview Claude follows when someone wants to write something down, or when a raw dump needs turning into a real note. Ask one question at a time, in plain language, pin down the fuzzy parts, then save a clean draft into the knowledge layer.
---

# The interview (grill)

Someone wants to capture how something works. Your job is to pull it out of their head with
simple questions, then write it down for them. They talk. You write.

This skill produces a DRAFT in `knowledge/`. It does not go on the trusted shelf yet. A
second person checks it later with `skills/check.md`.

Read `CLAUDE.md` first if you have not. The three rules and the three layers there always win.

## Step 1: Find the topic

Ask what they want to write down, in one line. Say it back in your own words so you both
agree on the topic before you dig in.

If they point you at something in `raw/` (a pasted chat, a photo note, a brain-dump), read
it first and use it as your starting point. But treat it as unchecked: confirm every part
with the person, and never copy a raw line in as true.

Then pick the closest shape from the `templates/` folder:

- A task with steps: `templates/sop.md`
- Who to call when something happens: `templates/who-to-call.md`
- A trick we use when the normal way fails: `templates/workaround.md`
- How a process works: `templates/how-it-works.md`
- What a new person needs: `templates/onboarding.md`

## Step 2: Ask one question at a time

- One question per message. Never stack two questions together. Wait for the answer.
- Plain words, in Thai. No jargon.
- Give your best guess as the first option, and say why. Let them just confirm it or fix it.
- Always allow "I do not know" or "I have to ask someone else" as an answer.

When they answer in their own words, say back what you understood in one sentence
("So you mean ..., is that right?") before you move on. Never quietly guess.

## Step 3: Pin down the fuzzy parts

Most rules are fuzzy at first. Sharpen them:

- If a rule has "usually" or "it depends", ask what it depends on, and get the exact case.
- If they give a number or a cut-off, ask "always that number?" and get the edge cases.
- Walk through one real example with real numbers and show it to them as a tiny list.
  Ask "is this what really happens?" A concrete example finds the gaps fast.

If they do not understand your question, the question was too hard, not the person. Make it
smaller, use a real example, and break it into two tiny yes-or-no questions.

## Step 4: The three hard cases

**They do not know.**
Do not delete the question and do not guess. Write it into the note as an open question:
what we do know, what is still missing, and who could answer it. Mark that part `LOW`.

**A new answer clashes with a note that already exists.**
Stop. Quote both, word for word, and say who said each. Ask which one is right now. Do not
merge them yourself, and do not quietly fix the old note. Keep both until a person decides.
(Rule 3.)

**No source.**
If they cannot say where a fact comes from and cannot point to who would know, do not write
it as true. Save it as an open question instead. (Rule 2.)

## Step 5: Write as you go

Write each part into the draft the moment it is clear. Do not save it all to the end, or a
stop halfway through loses everything.

Fill the frontmatter every time. Each fact goes in its own field (see `CLAUDE.md`, "What
goes at the top of every note"):

- `type`: the kind of note, matching the template you picked in Step 1 (`sop`,
  `who-to-call`, `workaround`, `how-it-works`, or `onboarding`).
- `title`: short, what the note is about.
- `updated`: today's date, written as `2026-08-21`.
- `confidence`: usually `MEDIUM` for a fresh draft (one person, not checked yet). Use `LOW`
  for the parts nobody could confirm.
- `source`: who told you. Just the person or role, not the date.
- `checked_by`: leave it blank. A fresh draft has not been checked yet; `skills/check.md`
  fills this in later.
- `tags`: a few short words for finding it later, or empty (`[]`) if none fit.

Keep the person's own words where they matter. If they said it well, save the sentence.

## Step 6: File it as a draft and log it

- Save the draft in `knowledge/`, one topic per file, with a short clear filename.
- At the bottom, add a small note: this is a draft, not checked yet, run `skills/check.md`
  before trusting it.
- Add one line to `log.md`: date, file, who told you, confidence, "captured (draft)".
- Read the draft back to them in a few lines and ask if anything is wrong. Fix it now,
  while they are still here.

## Step 7: Stop cleanly

If they say "last one" or run out of time, finish the draft you are on, save it, log it, and
stop. Do not start a new topic. Any open questions stay in the note for next time.

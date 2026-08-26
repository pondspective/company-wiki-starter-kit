---
name: check
description: Check a draft from the knowledge layer with a second person, then move it onto the trusted wiki shelf. This is the only way a note gets to be trusted.
---

# Check and publish a draft

A draft in `knowledge/` is one person's word, not yet confirmed. This skill gets a second
person to check it, then moves it to `wiki/` so the team can trust it.

Read `CLAUDE.md` first if you have not. The three rules and three layers there always win.

## Step 1: Pick a draft

Open a note from `knowledge/`. Best to check the ones people ask about most, or the ones a
task depends on. You do not have to check them in any order.

## Step 2: Read it back to the right person

Read the draft out loud, in a few short lines, to someone who really knows this topic. Best
if that is a different person from the one who first told it, or a lead. Ask after each part:
"Is this right? Anything missing? Anything you would say differently?"

## Step 3: Fix what is wrong

Correct the note as they talk. You do the typing. Keep their words where they matter.

If they disagree with something already on the trusted shelf in `wiki/`, do NOT quietly
change the old note. Put both versions side by side, say who said each, and ask which is
right now. (Rule 3.) Only after they decide do you update the trusted note.

## Step 4: Decide if it is ready

- If the main content is now confirmed: it is ready for `wiki/`.
- If one small corner is still unsure: that is fine. Leave that part as an open question
  marked `LOW`, and the rest can still go to `wiki/`.
- If most of it is still guesswork: leave it in `knowledge/` and note what still needs
  confirming. Do not force it onto the trusted shelf.

## Step 5: Move it to the trusted shelf

When it is ready:

- Raise `confidence` to `HIGH` (a second person has now checked it).
- Set `updated` to today's date.
- Put the checker's name in `checked_by`, and leave `source` as the person who first told
  it. For example: `source: พี่ต้อม` and `checked_by: พี่เมย์`.
- Remove the "this is a draft" note at the bottom.
- Move the file from `knowledge/` into `wiki/`.

## Step 6: Log it

Add one line to `log.md`: date, the new `wiki/` file, who told it and who checked it, `HIGH`,
"checked (moved to wiki)".

---
name: answer
description: How Claude answers a question from the wiki. Read the trusted shelf first, then drafts, then raw only if asked, and always say which shelf the answer came from.
---

# Answer a question

When someone asks a question, do not just answer from memory. Look in the folders, and be
honest about how much to trust what you find. This is what keeps trusted facts from getting
mixed up with guesses.

Read `CLAUDE.md` first if you have not. The three layers there are the whole idea.

## Step 1: Look in `wiki/` first

`wiki/` is the trusted shelf. If the answer is here, give it plainly. This is what the team
stands behind.

## Step 2: If it is not there, look in `knowledge/`

These are drafts, checked by only one person so far. You may use them, but say so clearly:
"I found this in a draft that has not been checked yet, so treat it as likely but not confirmed."
Then offer to get it checked (`skills/check.md`) so next time it is trusted.

## Step 3: Only look in `raw/` if they ask, or nothing else has it

`raw/` is the messy inbox that nobody has cleaned up. If you use anything from here, give the
strongest warning: "This is from an unchecked note in the inbox. It might be wrong." Then
offer to turn it into a real note with an interview (`skills/grill.md`).

## Step 4: If the answer mixes shelves, label each part

Do not blur them together. Say which part is trusted, which part is only a draft, and which
part is just an inbox note. The reader needs to know which is which.

## Step 5: If nothing has it, say so

Do not make up an answer. Say plainly that it is not written down anywhere yet, and offer to
capture it now with an interview (`skills/grill.md`). A clear "we do not know yet" is more
useful than a confident guess. (Rule 2.)

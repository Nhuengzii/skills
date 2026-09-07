---
name: dont-paste-the-brief
description: >
  Before accepting any agent deliverable — when output mirrors the brief, this
  chat/example, the crash site, or the latest human frame instead of the real job.
  Name the job, ban nearby junk, prove with a held-out check (channel / scope / cause).
---

# Don't paste the brief

**Problem:** the model treats nearby context (brief, criteria, this example, crash line, last chat message) as the answer.

**Fix:** name the real job → ban nearby junk → prove with a check that junk alone cannot pass.

One skill for this failure family. Keep it short.

## When to use

Before accepting any agent deliverable (UI, slides, docs, email, code, prompts, skills, bugfixes, research, decisions).

Fire when output sounds like a prompt, only works on this chat/example, is a lazy null-check/retry, or rubber-stamps the latest human frame.

## Every time (in order)

### 1. Name the job
One sentence: what must stay true for the *reader / next week / real cause* — not what was in the chat.

Examples:
- “User sees product text, not our build rules.”
- “Function handles any valid input shaped like X, not only the sample.”
- “Fix the producer that emits bad data, not the caller that crashes.”

Cannot write this sentence → stop.

### 2. Ban the nearby junk

| Nearby thing | Must not become |
|--------------|-----------------|
| Brief / criteria / “should / fallback / agent must” | UI, slide, email, doc, CLI user text |
| This file / ticket / sample / chat quote | The whole implementation or rule |
| Where it crashed | The full fix |
| User’s latest frame | Automatic agree + ship |

### 3. Prove it (pick what matches the job)

**A — Channel (copy / UI / slides / email)**  
Open the real artifact. No pasted brief. No process language unless the product teaches a rule on purpose. Rewrite or delete — do not soften.

**B — Scope (code / skills / prompts)**  
Invariant holds on ≥1 case **not** from this chat. Delete the special case once the general path works.

**C — Cause (bugfixes)**  
Name the cause layer in one line. Re-run the reproduce. No unlabeled nil-check / retry / test-disable as the main fix (label `temporary: symptom` if you must).

**Decisions / research**  
Survives swapping the frame/source. Disagree or state a condition — do not only agree.

Fail → rewrite. Missing proof = not done.

# German Teaching Material Generator

## What You Paste In

### 1. Current Error Report (Section B — Generator Feed)

```
[PASTE CURRENT ERROR REPORT HERE]
```

### 2. Previous Error Report (Section B — Generator Feed)

```
[PASTE PREVIOUS ERROR REPORT HERE]
```

---

## What You Will Receive

One markdown file used as a **warm-up review before the next practice set**.

Three parts:

- **PART 1 — Mini-Lessons:** Short targeted lessons built from your current errors. Each one starts from your actual wrong form, not an invented example.
- **PART 2 — Cheat Sheet:** Condensed reference tables you scan in 2 minutes before the next set.
- **PART 3 — Vocabulary Gap List:** Three sections — wrong/unknown words, word families, fixed phrases you keep breaking.

Total reading time: 10–15 minutes. This is a warm-up, not a study session.

---

## Core Instructions — Read Before Generating

You are working from structured error data only. The error report already contains everything: wrong forms, correct forms, categories, frequency, and recurrence across sets.

Your job:

1. Use CRITICAL errors first, then HIGH, then single-set errors.
2. Build every example from the actual wrong/correct forms in the report — never invent vocabulary.
3. Prioritize vocabulary and fixed phrase gaps — many of this student's errors come from not knowing the right word, not just misapplying a rule.
4. Keep everything short. One concept per lesson. One sentence per explanation. This student knows the rules — they need the correct forms to stick, not re-teaching.

**One absolute rule:** Every ❌ example must come directly from the FORM field in the error report. No invented errors.

---

## PART 1 — Mini-Lessons

### Format for each lesson:

```
## [Error Category Label]

❌ You wrote:   [wrong form — from FORM field in error report]
✅ Correct:     [correct form — from FORM field in error report]
💡 Why:         [one sentence — plain language, no jargon unless already in the report]

More examples:
• [correct example using vocabulary from the error report]
• [correct example using vocabulary from the error report]
• [correct example using vocabulary from the error report]
```

### Rules:

- One mini-lesson per error category — not one per individual wrong form
- If a category has multiple wrong forms (e.g. weil broken in 4 ways), pick the most representative one for ❌, use the others to build the "More examples" lines
- Order: CRITICAL errors → HIGH errors → single-set active errors
- Hard limit: **8 mini-lessons maximum** — merge minor single-set errors or drop them if they are not vocabulary-related
- The 💡 line must be one sentence. No sub-points. No lists inside a lesson.
- If an error is marked CRITICAL or seen in 3+ sets, add a 🔁 marker to the lesson header

---

## PART 2 — Cheat Sheet

Compact reference tables — scan before sitting down to the next set.

Generate **only the tables relevant to errors in the current report**. Skip any table where this student had no errors.

---

**Table: Negation Quick Reference** _(Include only if negation errors appear in the current report)_

|Situation|Use|Example from this set|
|---|---|---|
|Negating a verb/action|nicht|[example from report]|
|Negating a noun|kein/keine/keinen|[example from report]|
|Correcting after kein/nicht|sondern|[example from report]|
|Contradicting a kein-statement|doch|[example from report]|
|No longer|nicht mehr|[example from report]|
|Not yet — requires Perfekt|noch nicht + Perfekt|[example from report]|

---

**Table: Fixed Phrases — Location and Transport** _(Include only if location/transport errors appear in the current report)_

|Meaning|Correct German|❌ Wrong form from this set|
|---|---|---|
|at home|zu Hause|[from report if present]|
|at work|bei der Arbeit|[from report if present]|
|by bike|mit dem Fahrrad|[from report if present]|
|by car|mit dem Auto|[from report if present]|

---

**Table: Subordinate Clauses — Verb Goes Last** _(Include only if weil/wenn/dass errors appear in the current report)_

|Conjunction|Correct example|❌ Your version|
|---|---|---|
|weil|[from report]|[from report]|
|wenn|[from report]|[from report]|

---

**Table: seit — Duration** _(Include only if seit errors appear in the current report)_

|Structure|Correct|❌ Wrong|
|---|---|---|
|Statement — ongoing|seit + present tense|[from report]|
|Question — how long|Seit wie vielen Jahren…?|[from report]|

---

**Table: Adjective Endings** _(Include only the cases that were wrong in the current report — not all 48 combinations)_

|Article type|Gender/Case|Ending|Example from this set|
|---|---|---|---|
|[only wrong cases]||||

---

### Cheat sheet rules:

- Every example cell uses vocabulary from the error report — no abstract placeholders
- If a table would exceed 8 rows, split it
- No prose between tables — headers and tables only
- If an error category has no natural table format, skip it — do not force it into Part 2

---

## PART 3 — Vocabulary Gap List

Three sections. Clean lists only — no prose, no explanations longer than a parenthetical.

---

### Section A: Words You Used Wrong or Didn't Know

Built from: FORM fields where the error is clearly a vocabulary mistake (wrong word chosen, noun used instead of adjective, English word used, word simply absent).

|Your version|Correct German|English meaning|Notes|
|---|---|---|---|
|[from report]|[from report]|[translation]|[noun vs. adjective / register / fixed phrase / _(unknown)_]|

Rules:

- Only include words that caused an actual error in the current report
- Mark with _(unknown)_ in Notes if the student clearly didn't know the word at all (wrote English, left blank, or used a completely unrelated word)
- One-word Notes only — no full sentences

---

### Section B: Word Families

For each word where the student confused forms (used noun instead of adjective, used infinitive instead of conjugated verb, etc.), show the relevant family.

Format:

```
Root: [WORD]

| Form | German | Example |
|---|---|---|
| adjective | … | … |
| noun | … | … |
| verb | … | … |
```

Rules:

- Only generate families for roots where form-confusion caused an error in the current report
- Maximum 5 families per output
- Only include forms up to B1 level — skip advanced derivations
- Examples must use vocabulary from the error report

---

### Section C: Fixed Phrases You Keep Breaking

Memorized units — not built by rules. Do not explain them grammatically.

|Correct phrase|Meaning|❌ Your version||
|---|---|---|---|
|[from report]|[English]|[from report]|🔁 if seen in 3+ sets|

Rules:

- Include only phrases that appear as errors in the current report
- Add 🔁 if the phrase has been wrong across 3 or more sets (visible in FREQUENCY field of report)
- No grammar notes — these are memory items
- If a phrase was correct this set, do not include it even if it was wrong before

---

## Formatting Rules

- Total length: 600–900 words (not counting table content)
- Part headers: `# PART [N] — [NAME]`
- Mini-lesson headers: `## [Topic Label]`
- No exercises — review material only
- No word banks
- No praise, no encouragement, no filler
- One file only

---

## Output

Generate the teaching material now based on the two error reports above. No preamble. No explanation. Start directly with PART 1.
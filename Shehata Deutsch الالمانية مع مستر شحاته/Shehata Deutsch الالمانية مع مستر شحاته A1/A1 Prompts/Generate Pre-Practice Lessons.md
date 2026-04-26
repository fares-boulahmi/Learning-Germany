# German Teaching Material Generator

## What You Paste In

### 1. Your Written Answers (current set)

```
[PASTE YOUR ANSWERS HERE]
```

### 2. Answer Key (current set)

```
[PASTE ANSWER KEY HERE]
```

### 3. Error Report (current set — Section B Generator Feed is enough)

```
[PASTE ERROR REPORT HERE]
```

---

## What You Will Receive

One markdown file used as a **warm-up review before the next practice set**.

It contains three parts:

- **PART 1 — Mini-Lessons:** Short targeted lessons built from your specific errors. Not generic grammar explanations — each lesson uses your actual wrong sentences as the starting point.
- **PART 2 — Cheat Sheet:** Condensed reference tables you scan in 2 minutes before sitting down to the next set.
- **PART 3 — Vocabulary Gap List:** Three sections — wrong/unknown words, word families, and fixed phrases you keep breaking.

Total reading time: 10–15 minutes maximum. This is a warm-up, not a study session.

---

## Core Instructions — Read Before Generating

You are analyzing the gap between what the student wrote and what was correct. Your job is NOT to re-explain all of German grammar. Your job is to:

1. Extract only what this student got wrong in this set.
2. Build the shortest possible explanation that closes each specific gap.
3. Make every example use vocabulary from the student's own errors — not invented sentences.
4. Prioritize vocabulary and fixed phrase gaps over abstract grammar rules, because the student's errors are often caused by not knowing the right word, not just not knowing the rule.

**One absolute rule:** If the student wrote something wrong, the mini-lesson must show:

- Exactly what they wrote
- Exactly what was correct
- Why in one sentence maximum
- Three more correct examples using the same rule

No long explanations. No numbered lists of sub-rules. One concept, one correction, three examples, done.

---

## PART 1 — Mini-Lessons

### Format for each lesson:

```
## [Grammar/Vocabulary Topic — short label]

❌ You wrote:     [exact wrong sentence from student's answers]
✅ Should be:    [correct version]
💡 Why:          [one sentence only — the rule in plain language]

More examples:
• [correct example sentence 1]
• [correct example sentence 2]
• [correct example sentence 3]
```

### Rules for building mini-lessons:

- Generate one mini-lesson per **error category** from the error report — not one per individual mistake
- Use the student's actual wrong sentences as the ❌ example — never invent a fake error
- If a category has multiple errors (e.g. weil-clause broken in 4 places), pick the most representative one for the ❌ line, then use the others as the "more examples" if useful
- Order lessons from CRITICAL errors first → HIGH errors → single-set errors last
- Hard limit: maximum 8 mini-lessons total. If there are more error categories, merge the minor ones or skip the ones that are single-set and not vocabulary-related
- The "💡 Why" line must be in plain language — no grammatical terminology unless the student already uses it (e.g. "Perfekt", "dative" are fine if they appear in the error report)

---

## PART 2 — Cheat Sheet

A set of compact reference tables the student scans before sitting down to the next practice set.

### Required tables — generate ALL of these if relevant to this set's errors:

**Table 1: Negation Quick Reference**

|Situation|Use|Example|
|---|---|---|
|Negating a verb/action|nicht|Er kommt nicht.|
|Negating a noun (no/none)|kein/keine/keinen|Ich habe kein Geld.|
|Correcting after kein/nicht|sondern (not aber)|Kein Hund, sondern eine Katze.|
|Contradicting a kein-statement|doch|— Kein Glück. — Doch, viel Glück.|
|No longer|nicht mehr|Er arbeitet nicht mehr hier.|
|Not yet (requires Perfekt)|noch nicht|Ich habe es noch nicht gekauft.|

_(Populate the example column with vocabulary from the student's actual set — not generic examples)_

**Table 2: Fixed Phrases — At/To/From Places**

|Meaning|Correct German|Common Wrong Form|
|---|---|---|
|at home|zu Hause|~~im Haus~~|
|at work|bei der Arbeit|~~zu Arbeit~~|
|by bike|mit dem Fahrrad|~~mit Fahrrad / bei das Fahrrad~~|
|by car|mit dem Auto|~~mit Auto~~|
|to Hamburg (directed)|nach Hamburg|~~zu Hamburg~~|

_(Add or remove rows based on what appeared in this set's errors — only include phrases that were actually wrong)_

**Table 3: weil / wenn / dass — Verb Goes Last**

|Conjunction|Example|❌ Common Error|
|---|---|---|
|weil|…weil er müde **ist**|~~weil er ist müde~~|
|wenn|…wenn ich komme,|~~wenn komme ich,~~|
|dass|…dass sie arbeitet|~~dass sie arbeitet~~ (usually correct)|

_(Only include rows where this student actually made errors — remove any rows that were clean)_

**Table 4: seit — How Long**

|Structure|Correct|Wrong|
|---|---|---|
|How long (statement)|seit + present tense|~~seit + past tense~~|
|How long (question)|Seit wie vielen Jahren…?|~~Seit wie viele Jahren…?~~|
|Still happening now|schon included|~~schon omitted~~|

**Table 5: Adjective Endings Snapshot** Only include cases that were wrong in this set. Use a minimal table — not all 48 combinations.

|Article type|Gender/Case|Ending|Example|
|---|---|---|---|
|definite (der/die/das)|plural, nominative|-en|die teuren Eier|
|indefinite (ein)|masculine, nominative|-er|ein guter Käse|
|no article|feminine, nominative|-e|frische Butter|

_(Only include rows where this student made errors — remove clean rows)_

### Cheat sheet rules:

- Every example cell must use vocabulary from this set — no abstract placeholders
- Tables must fit on one screen — if a table would be longer than 8 rows, split into two smaller ones
- Do not add explanatory prose between tables — headers and tables only
- If an error category has no natural table format, skip it — do not force prose into Part 2

---

## PART 3 — Vocabulary Gap List

Three sections. Each section is a clean list — no prose, no explanations longer than a parenthetical note.

---

### Section A: Words You Used Wrong or Didn't Know

Format:

```
| Your version | Correct German | English meaning | Notes |
|---|---|---|---|
| gesundheit nicht | nicht gesund | not healthy | gesund = adjective; Gesundheit = noun |
| der Manager | der Chef | the boss/manager | Chef is standard in German workplace context |
```

Rules:

- Only include words that caused an actual error — not every word in the set
- The "Notes" column: one short parenthetical only — noun vs. adjective, register note, or "fixed phrase"
- If the student simply didn't know the word (left blank or wrote English), flag it with _(unknown)_ in the Notes column

---

### Section B: Word Families

For each word the student misused (noun used where adjective needed, wrong form of a known root, etc.), show the full family — but only the forms relevant to A2/B1 level.

Format:

```
Root: GESUND

| Form | German | Example |
|---|---|---|
| adjective | gesund | Er ist gesund. |
| noun | die Gesundheit | Gesundheit ist wichtig. |
| adverb | gesundheitlich | Das ist gesundheitlich bedenklich. |
| comparative | gesünder | Sie ist gesünder als er. |
```

Rules:

- Only generate word families for roots where the student showed confusion between forms (used the noun where the adjective was needed, etc.)
- Maximum 5 word families per set — pick the most important ones
- Skip forms that are clearly above B1 level

---

### Section C: Fixed Phrases You Keep Breaking

A clean two-column list of phrases that are memorized units — not built by rules.

Format:

```
| Correct phrase | Meaning | ❌ Your version |
|---|---|---|
| zu Hause | at home | im Haus |
| bei der Arbeit | at work | zu Arbeit |
| mit dem Fahrrad | by bike | mit Fahrrad |
| keine … mehr | none left | nie / kein |
| eine eigene Wohnung | one's own apartment | seine Wohnung |
```

Rules:

- Include ONLY phrases that appeared as errors in this set
- If a phrase has been wrong in 3+ sets (visible in error report), mark it with 🔁 in a fourth column
- No grammar explanations — these are memory items, not rule applications
- If a phrase was correct this set, do not include it even if it was wrong before

---

## Formatting Rules

- Total length: 600–900 words (not counting table content)
- Part headers: `# PART [N] — [NAME]`
- Mini-lesson headers: `## [Topic Label]`
- No word banks
- No exercises — this is review material, not a practice set
- No praise, no encouragement, no filler sentences
- Output is one file only

---

## Output

Generate the teaching material now based on the inputs above. No preamble. No explanation. Start directly with PART 1.
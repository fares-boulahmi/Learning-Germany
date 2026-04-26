# German Practice Set Generator — v2

## Who This Is For

A learner currently at high A1/low A2, crashing toward B1.

- Already completed teacher lessons + exercises before this set runs
- ~4 hours/day total for grammar work
- Goal: pass B1 exam — grammar must **stick**, not just be recognized
- Each set is done once, never repeated — no recycling content across sets

---

## What You Receive as Input

### 1. Error Report

```
[PASTE ERROR REPORT HERE]
```

### 2. Lesson + Exercise Summary

```
[PASTE LESSON SUMMARY HERE]
```

---

## Core Philosophy — Read Before Generating

**The student already knows the rules. The teacher already explained them. The teacher exercises already drilled them once.**

This set does NOT re-explain rules. It does NOT scaffold. It does NOT hold hands.

Its only job is to force the student to **produce correct German under pressure**, combining multiple rules at once, in contexts the teacher did not use.

**Three principles:**

1. **Pressure over comfort** — every exercise should feel slightly too hard. If the student can do it easily, it is not useful.
2. **Production over recognition** — filling a blank from a word bank teaches nothing. Building a sentence from scratch teaches everything.
3. **Integration over isolation** — never test one rule alone. Every exercise should require at least two grammar rules simultaneously.

---

## What to Generate

### Two markdown files:

---

## FILE 1: `German Practice Set [X].md`

---

### Structure: 5 blocks only. No more.

---

### BLOCK 1 — Error Ambush (30% of set)

**Purpose:** Take the student's active critical errors and disguise them inside **new** vocabulary and **new** contexts they haven't seen before — so they cannot rely on pattern memory from teacher exercises.

**Format rules:**

- No labels like "⚠️ ERROR TARGET" on the exercises themselves — the student must find the trap alone
- After the answer key: reveal which trap was hidden where
- Mix ALL critical errors together in the same exercises — do not separate them by error type
- Use ONLY vocabulary from the current lessons (not old lessons)

**Exercise types to use (pick 2–3 per block, never repeat the same type twice in one set):**

- Paragraph with 12–18 errors hidden — student finds and rewrites
- 15–20 sentence translations English→German with traps embedded
- Dialogue reconstruction — jumbled sentences, student reorders AND fixes errors
- Sentence transformation — change person/tense/register while keeping meaning

**Length:** 400–500 words of exercise content

---

### BLOCK 2 — Grammar Under Pressure (25% of set)

**Purpose:** Test the new lesson grammar at B1-adjacent difficulty — more complex sentences, subordinate clauses, real-world ambiguity.

**Format rules:**

- No hint labels. No "use modal verb here."
- Sentences should be long enough to require holding multiple rules in mind at once
- At least one exercise must combine new lesson content WITH a previously known grammar rule
- At least one exercise must require the student to choose between two similar structures (e.g. seit vs. vor, doch vs. ja, wohin vs. wo)

**Exercise types to use (pick 2–3):**

- Sentence building from 5–7 scrambled words (no hints)
- Translate 12–15 sentences where each one contains a decision point
- Error detection in a full paragraph (errors not counted — student must find them all)
- Fill-in-the-blank paragraph — NO word bank, NO hints, blanks only

**Length:** 350–450 words of exercise content

---

### BLOCK 3 — Speed Production (15% of set)

**Purpose:** Force fast, automatic production. B1 exams have time pressure. The student must build correct German quickly without stopping to think about every rule.

**Format:**

- 20–25 very short prompts
- Student writes ONE complete correct German sentence per prompt
- No scaffolding at all
- Prompts mix: translations, "say this in German", "make a question from this statement", "contradict this with doch"
- Strict rule: every sentence must use at least one grammar rule from the current lessons OR error report

**Length:** ~200 words of prompts (answers will be much longer)

---

### BLOCK 4 — Integrated Production Task (20% of set)

**Purpose:** One substantial writing task that forces the student to use everything at once.

**Format:** Choose ONE of the following based on what the lessons covered:

- Formal letter or email (16–20 sentences)
- Mixed-register dialogue (20–26 exchanges — two people, different formality levels)
- Descriptive paragraph + response dialogue combined

**Checklist provided — but lean:** Give the student ONLY a bullet list of 8–10 grammar/vocabulary requirements they must include. No sentence starters. No "write X about Y." The scenario is stated in one sentence and nothing more.

**Errors to avoid list:** Include 5–6 specific traps from the error report. No explanations — just the wrong form → correct form.

**Example of lean checklist format:**

```
Scenario: You are applying for a job at a German hospital. Write the application email.

Must include:
- seit + present tense (duration)
- one doch response (embedded in a reference to a previous conversation)
- two modal verbs with infinitive at end
- one feminine profession with correct article
- your birthday as an ordinal date
- schon or erst
- wo/wohin/woher question
- formal Sie register throughout

Do NOT write:
- bis um → bis only
- der Lehrerin → die Lehrerin
- Ich kann komme → Ich kann kommen
- Er bin → Er ist
- halb dreizehn → halb eins
```

**Length:** 200–250 words of task description + checklist

---

### BLOCK 5 — B1 Bridge (10% of set)

**Purpose:** Introduce one concept that is slightly beyond the current lesson level but directly useful for B1. This is not tested heavily — it is exposure. The student will see it again in future sets.

**Format:**

- Brief rule explanation (5–8 lines MAX — no long grammar lectures)
- 6–8 example sentences showing the rule in action
- 4–5 exercises where the student tries to apply it
- Label this block clearly: **"B1 Preview — this will appear again in future sets"**

**What to introduce:** Choose based on what the current lessons are approaching. Good candidates:

- Subordinate clause word order (weil, dass, obwohl)
- Accusative vs. dative with two-way prepositions (already started with stellen/legen)
- Adjective endings (nominative first)
- Perfekt tense (haben/sein + past participle)
- Reflexive verbs in context
- Coordinating vs. subordinating conjunctions

**Length:** 200–300 words

---

### Formatting Rules for FILE 1

- Total set length: **1400–1800 words** (exercises only — not counting answer blanks)
- Section headers: `### Block [N]: [Name]`
- Answer blanks: use `⇒` with a line, nothing else
- No ⚠️ labels on exercises (only in answer key)
- No word banks anywhere
- No grammar reminders inside exercises (those belong in the answer key)

---

## FILE 2: `Answer Key — Set [X].md`

### Structure:

For each block:

```
## Block [N]: [Name]

### Exercise [N.X]
1. [correct answer]
   - ⚠️ Trap: [which error this targeted] — [one sentence explanation]
2. [correct answer]
[...]
```

**Rules for the answer key:**

- Every answer that involves a trap from the error report → mark with ⚠️ and name the error
- Alternative acceptable answers listed where they exist
- For the integrated production task: provide a **model answer** (full correct version) + a **correction checklist** the student can use to self-grade
- For the B1 Bridge: provide all correct answers + one extra example sentence not in the exercises
- Keep explanations SHORT — one sentence per note maximum. The student knows the rule. They just need to see the correct form.

**Total answer key length:** 800–1200 words

---

## Quality Control — Run Before Outputting

### Efficiency check:

- [ ] No exercise type appears more than once across the whole set
- [ ] No vocabulary or grammar structure repeated from the previous set's exercises
- [ ] Total word count 1400–1800 (FILE 1) and 800–1200 (FILE 2)
- [ ] No word banks anywhere in FILE 1

### Targeting check:

- [ ] Every critical error from the report appears at least twice in Block 1
- [ ] Block 2 uses ONLY grammar from the current lessons
- [ ] Block 3 prompts are genuinely fast — student should feel time pressure
- [ ] Block 4 task is realistic and requires genuine German production
- [ ] Block 5 concept is one step ahead of current lessons — not two steps

### Difficulty check:

- [ ] Would a strong A2 student struggle with Block 1? If not, add complexity.
- [ ] Does Block 2 require holding two rules in mind at once? If not, combine.
- [ ] Is Block 4 impossible without knowing the lesson content? Good. That's the point.
- [ ] Does Block 5 feel slightly unfamiliar but logical? Good.

### Trap check (Block 1 only):

- [ ] Are traps hidden inside new vocabulary the student hasn't drilled before?
- [ ] Are multiple error types combined in single sentences?
- [ ] Is there NO signal to the student that a trap is coming?

---

## What This Set Does NOT Do

- Does not re-explain grammar rules the teacher already taught
- Does not use word banks
- Does not label traps during exercises
- Does not repeat exercise types within a set
- Does not recycle content from previous sets
- Does not have more than 5 blocks
- Does not have more than 2 creative tasks
- Does not exceed 1800 words in FILE 1

---

## Output

Generate both files now based on the error report and lesson summary above.  
FILE 1 first, then FILE 2.  
No preamble. No explanation. Start directly with the content.
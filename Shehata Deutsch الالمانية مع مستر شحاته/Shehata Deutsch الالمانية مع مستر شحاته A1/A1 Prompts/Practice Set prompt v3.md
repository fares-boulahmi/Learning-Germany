# German Focused Consolidation Set — Prompt

---

## What This Is

A targeted drilling set that runs **after** you've already done the lesson exercises once. It does not re-teach. It does not scaffold. It forces you to produce correct German under moderate pressure using only grammar you've already studied and vocabulary you already know.

---

## What You Provide as Input

### 1. Lesson Notes (Part 1 output from Lesson Processor)

```
[PASTE LESSON NOTES HERE]
```

### 2. Error Report

```
[PASTE ERROR REPORT HERE]
```

### 3. Known Word List

```
[PASTE KNOWN WORD LIST HERE]
```

---

## Core Rules — Read Before Generating

**The student has read the lesson notes and knows the rules. They have not done any exercises yet on this material. This set is the first and only drilling pass.**

This is a volume-based consolidation set. The goal is automaticity through repetition, not exam-pressure performance. Each exercise targets a small number of rules clearly. The student should finish each item feeling like they owned it — or clearly see where they didn't.

**Three non-negotiable principles:**

1. **Lesson grammar as anchor** — the current lesson's grammar theme shapes the exercises, but previously learned grammar (subordinate clauses, negation, modal verbs, Perfekt, etc.) must appear naturally throughout. Never test only one rule in isolation — always combine at least 2.
2. **Error targeting embedded, not labeled** — every critical and active error from the report must appear inside exercises without flagging. The student does not know a trap is coming.
3. **No creative writing tasks** — no letters, no emails, no dialogue composition. Pure grammar production only.

---

## Vocabulary Rule (Strict — No Exceptions)

- Use **only** words from the provided known word list
- Connectors and function words are always free regardless of word list: _weil, obwohl, dass, aber, sondern, doch, dann, danach, davor, nachdem, während, als, wenn, deshalb, trotzdem, außerdem, zuerst, schließlich, vor, unter, über, durch, gegen, ohne, um, zwischen, neben, hinter, nämlich,_ etc.
- If a word is not in the known list and is not a function word, do not use it. No exceptions. No inline marking. Rewrite the sentence to avoid it.

---

## Exercise Count

Always generate exactly **20 exercises**. No more, no fewer.

---

## Exercise Types — Available Pool

Types may repeat across the 20 exercises. Never use the same type more than **4 times** in one set.

|Code|Type|Description|
|---|---|---|
|TR|Translation EN→DE|8–10 sentences, each with exactly one grammar decision point embedded|
|SB|Sentence building|5–7 scrambled word groups (5–7 words each), student assembles correct sentence|
|ED|Error detection paragraph|One continuous paragraph, 8–12 errors hidden, student rewrites entirely corrected|
|FI|Fill-in paragraph|Continuous text, blanks only — no word bank, no hint labels|
|TX|Sentence transformation|6–8 sentences, each requires one specific structural change (change tense / negate / subordinate / pronoun replacement)|
|ST|Subordinate clause construction|6–8 sentence pairs, student combines using a given connector|
|NC|Negation correction|6–8 sentences each with one negation error, student identifies and rewrites|
|TP|Tense-switching paragraph|Short paragraph given in Präsens, student rewrites fully in Perfekt (or reverse)|
|QA|Question-answer production|6–8 questions, student writes complete grammatically correct answers using own words|
|MX|Mixed correction|8–10 isolated sentences, one error each, student identifies and fixes|

---

## Difficulty Level

Target: a student who knows the rules individually but is still building automaticity. Each exercise should feel achievable but require genuine attention.

- Sentences are shorter than exam level — one clear grammar challenge per item
- Each exercise combines exactly **2 grammar rules** — no more
- At least 4 exercises must combine the current lesson grammar with a rule from a previous topic
- At least 2 exercises must use subordinate clause structure (weil / obwohl / dass / wenn / als)
- At least 1 exercise must require the student to choose between two structures they commonly confuse based on their error report

Specific difficulty markers:

- No fill-in-the-blank may provide the infinitive as a hint inside the blank
- No translation may include word order hints through bracketing
- No error detection may state how many errors exist
- Transformation tasks require only one change per sentence — the rest stays identical

---

## How to Select Exercises

1. Look at the critical errors in the report — these must appear in at least **3 different exercises** each
2. Look at the active errors — these must appear in at least **2 exercises** each
3. Look at the lesson grammar focus — at least **5 exercises must directly require the lesson's grammar**
4. Distribute the 20 exercises across at least **6 different exercise types**
5. No type may appear more than 4 times

---

## Output Format

Return everything in a single message in this exact structure:

```markdown
# Consolidation Set — [Lesson Range / Topic]

---

## Part 1 — Exercises

### Exercise 1 — [Type Name] *(Grammar focus: [2 rules])*
[content]
⇒

### Exercise 2 — [Type Name] *(Grammar focus: [2 rules])*
[content]
⇒

[...continue to Exercise 20]

---

## Part 2 — Answer Key

**Exercise 1**
1. [correct answer]
   — ⚠️ [error name if targeted]: [one-line note]
2. [correct answer]
[...]

**Exercise 2**
[...]
```

**Format rules:**

- Return directly in chat as markdown — no file created
- Two clearly labeled sections: Part 1 (all 20 exercises) then Part 2 (full answer key)
- Section headers: `### Exercise [N] — [Type]`
- Grammar focus label after every header: always exactly 2 rules listed
- Answer blank: `⇒` on its own line, nothing else
- Answer key: in Part 2, after all exercises
- Error traps in key: marked `⚠️` with name of the error and a one-sentence note
- Alternative acceptable answers listed where they exist
- No ⚠️ labels anywhere in Part 1

---

## What This Set Does NOT Do

- Does not re-explain any grammar rule
- Does not use word banks anywhere
- Does not label traps during exercises
- Does not introduce vocabulary outside the known word list
- Does not include any creative writing task
- Does not produce any exercise that targets only one rule in isolation
- Does not use the same exercise type more than 4 times
- Does not go above or below 20 exercises
- Does not test any resolved error from the report
- Does not create a file — returns in chat as markdown only

---

## Quality Check — Run Before Outputting

- [ ] Exactly 20 exercises generated
- [ ] At least 6 different exercise types used
- [ ] No type used more than 4 times
- [ ] Every critical error appears in at least 3 exercises
- [ ] Every active error appears in at least 2 exercises
- [ ] At least 5 exercises directly test the current lesson grammar
- [ ] Every exercise combines exactly 2 grammar rules
- [ ] At least 4 exercises combine lesson grammar with a previous topic
- [ ] At least 2 exercises use subordinate clause structure
- [ ] At least 1 exercise forces a choice between two commonly confused structures
- [ ] No vocabulary outside the known word list — no exceptions
- [ ] No word banks anywhere
- [ ] No error labels in Part 1
- [ ] No fill-in hint gives the infinitive inside the blank
- [ ] Answer key complete with ⚠️ notes on all targeted items
- [ ] No creative writing task
- [ ] Output is markdown in chat — no file created

---

_Generate the set now. No preamble. Start directly with Exercise 1._
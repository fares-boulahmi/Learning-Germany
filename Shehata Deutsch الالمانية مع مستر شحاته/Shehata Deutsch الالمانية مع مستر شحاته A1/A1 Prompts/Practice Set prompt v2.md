# German Focused Consolidation Set — Prompt

---

## What This Is

A targeted drilling set that runs **after** you've already done the lesson exercises once. It does not re-teach. It does not scaffold. It forces you to produce correct German under exam pressure using only grammar you've already studied and vocabulary you already know.

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

But this is not a beginner drill. The student is building toward B1/B2 exam mastery. They already know most rules from previous sets. The current lesson grammar is the _thematic anchor_ — it gives the exercises their context — but every exercise should treat the student as someone who is expected to control all previously learned grammar simultaneously, not just the lesson topic.

**Three non-negotiable principles:**

1. **Lesson vocabulary as anchor, not cage** — the current lesson's grammar theme shapes the exercises, but other grammar rules the student has already encountered (subordinate clauses, negation, modal verbs, connectors, Perfekt, imperatives, etc.) must appear naturally throughout. The student should never feel "this exercise is only about one thing."
2. **Error targeting embedded, not labeled** — every critical and active error from the report must appear inside exercises without flagging. The student does not know a trap is coming.
3. **No creative writing tasks** — no letters, no emails, no dialogue composition. Pure grammar production only.

---

## Vocabulary Rule (Strict)

- Use **only** words from the provided known word list + new words introduced in the lesson's Part 2
- Connectors and function words are always free to use regardless of word list: _weil, obwohl, dass, aber, sondern, doch, dann, danach, davor, nachdem, während, als, wenn, deshalb, trotzdem, außerdem, zuerst, schließlich, vor, unter, über, durch, gegen, ohne, um, zwischen, neben, hinter, nämlich,_ etc.
- If you must use a content word not in the known list, mark it immediately after with `[= meaning]` inline — this is the only exception and must be rare

---

## Exercise Count

Scale to lesson and error count:

|Lesson count|Critical errors|Exercise count|
|---|---|---|
|1–2|any|7|
|3–4|≤ 4|7|
|3–4|5+|8|
|5+|any|9|

Never go below 7. Never go above 9.

---

## Exercise Types — Available Pool

Pick from this pool. **Never repeat the same type twice in one set.**

|Code|Type|Description|
|---|---|---|
|TR|Translation EN→DE|10–15 sentences, each with exactly one grammar decision point embedded|
|SB|Sentence building|6–8 scrambled word groups (5–8 words each), student assembles correct sentence|
|ED|Error detection paragraph|One continuous paragraph, 10–15 errors hidden, student rewrites entirely corrected|
|FI|Fill-in paragraph|Continuous text, blanks only — no word bank, no hint labels|
|TX|Sentence transformation|8–10 sentences, each requires one specific structural change (change tense / negate / subordinate / change register)|
|ST|Subordinate clause construction|8–10 sentence pairs, student combines using a given connector — connector is given, nothing else|
|NC|Negation correction|8–10 sentences each with one negation error (aber/sondern, nicht/kein, noch/schon etc.), student identifies and rewrites|
|TP|Tense-switching paragraph|Short paragraph given in Präsens, student rewrites fully in Perfekt (or reverse)|
|QA|Question-answer production|8–10 questions given, student writes complete grammatically correct answers using own words — no answer scaffolding|
|MX|Mixed correction|10–12 isolated sentences, one error each, student identifies and fixes|

---

## How to Select Exercises

1. Look at the critical errors in the report — these must appear in at least **2 different exercises** each
2. Look at the active errors — these must appear in at least **1 exercise** each
3. Look at the lesson grammar focus — at least **3 exercises must directly require the lesson's grammar** (not just error-targeting)
4. Every exercise must require **at least 2 grammar rules simultaneously** — never test one rule in isolation
5. At least **1 exercise must use subordinate clauses** (weil / obwohl / dass / wenn / als / nachdem etc.) as the structural frame

---

## Difficulty Level

Target: a student who knows all the rules _in isolation_ but hasn't yet made them automatic together. This set should feel like it's testing whether you truly own the grammar, not whether you recognize it.

- Harder than a standard A2/B1 drill
- Sentences should be long enough that the student must hold 2–3 rules in mind simultaneously
- At least 3 exercises must combine the current lesson grammar with a rule from a _previous_ topic (Perfekt + subordinate clause, modal + negation, imperative + separable verb, etc.)
- No exercise should feel like it belongs to "Folge 69" specifically — it should feel like real German that happens to use Perfekt, or uses _-ieren_ verbs, or uses _sein_ Perfekt — naturally embedded

Specific difficulty markers:

- No fill-in-the-blank may provide the infinitive as a hint inside the blank
- No translation may include word order hints through bracketing
- No error detection may state how many errors exist
- At least one exercise must require the student to choose between two similar structures they commonly confuse (e.g. _seit_ vs. _vor_, _aber_ vs. _sondern_, _noch nicht_ + Perfekt vs. Präsens, _bekommt_ vs. _kommt_)


---

## Output Format

```markdown
# Consolidation Set — [Lesson Range / Topic]

---

### Exercise 1 — [Type Name] *(Grammar focus: [rules])*
[content]
⇒

### Exercise 2 — [Type Name] *(Grammar focus: [rules])*
[content]
⇒

[...continue to 7–9]

---

<details>
<summary>Answer Key</summary>

**Exercise 1**
1. [correct answer]
   — ⚠️ [error targeted, if any]: [one-line note]
2. [correct answer]
[...]

**Exercise 2**
[...]

</details>
```

**Format rules:**

- Section headers: `### Exercise [N] — [Type]`
- Grammar focus label after header: always present, lists the 2+ rules being combined
- Answer blank: `⇒` on its own line, nothing else
- Answer key: inside a `<details>` collapse block
- Error traps in key: marked `⚠️` with name of the error from the report and a one-sentence note
- Alternative acceptable answers listed where they exist
- No ⚠️ labels visible anywhere in the exercises themselves — only in the answer key

---

## What This Set Does NOT Do

- Does not re-explain any grammar rule
- Does not use word banks anywhere
- Does not label traps during exercises
- Does not repeat an exercise type within one set
- Does not introduce vocabulary outside the known list (except inline-marked exceptions)
- Does not include any creative writing task (no letters, emails, dialogues, essays)
- Does not exceed 9 exercises
- Does not go below 7 exercises
- Does not test any resolved error from the report
- Does not produce any exercise that targets only one rule in isolation

---

## Quality Check — Run Before Outputting

- [ ] Every critical error appears in at least 2 exercises
- [ ] Every active error appears in at least 1 exercise
- [ ] At least 3 exercises directly test the current lesson grammar
- [ ] Every exercise requires 2+ grammar rules simultaneously
- [ ] At least 1 exercise uses subordinate clause structure
- [ ] No exercise type appears more than once
- [ ] No vocabulary outside known list (exceptions inline-marked)
- [ ] No word banks anywhere
- [ ] No error labels visible in exercise body
- [ ] Exercise count matches the scaling table
- [ ] No fill-in hint gives the infinitive form inside the blank
- [ ] Answer key is complete with ⚠️ trap notes on all targeted items
- [ ] No creative writing task in the set

---

_Generate the set now. No preamble. Start directly with Exercise 1._

---

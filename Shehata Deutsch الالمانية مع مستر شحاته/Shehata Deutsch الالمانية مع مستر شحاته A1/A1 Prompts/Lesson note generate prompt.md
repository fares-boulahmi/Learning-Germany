# Lesson Processor — German Grammar (A1→B1 Path)

## Your Job

You receive a raw copy-paste from a German grammar PDF.
It may contain **multiple lessons** (anywhere from 1 to 7+).
It may be messy: Arabic mixed in, broken formatting, repeated headers, OCR artifacts, duplicate exercises.

You will output **one clean Markdown file** with exactly **two parts**.

---

## How to Detect Lesson Boundaries

A new lesson starts when you see any of:
- A new "Folge" or episode number (e.g. `Folge 36`, `Folge 37`)
- A new bold/uppercase title that introduces a new grammar topic
- A clear thematic break (e.g. Nominativ → Akkusativ → Dativ)

If boundaries are ambiguous, group by grammar topic, not by page.

---

## PART 1 — Clean Lesson Notes

Process each detected lesson separately, in order.
All lessons go into one Part 1, each under its own `###` heading.

**Rules:**
- Keep Arabic where it directly translates a grammar term or explains a concept. Remove Arabic that is filler, page notices, or copyright lines.
- Remove ALL of the teacher's original exercises (Übung 1, Übung 2, etc.).
- Remove page numbers, copyright notices, publisher warnings.
- Restructure into clean Markdown: `###` for lesson headers, `####` for subsections, tables for grammar paradigms, bullet points for rules, blockquotes for example sentences.
- Keep every grammar table — format as Markdown tables.
- Keep all example sentences, labeled under the rule they illustrate.
- Do NOT add explanations the teacher didn't give. Clean and restructure only.

---

## PART 2 — Combined Practice Exercises

Generate **a maximum of 7 exercises total** across ALL lessons.

**Core rule: every exercise must combine concepts from at least 2 different lessons.**
Do not write an exercise that tests only one lesson in isolation.
The goal is to force the student to hold multiple rules in mind at once.

**Difficulty target:** Harder than the teacher's original exercises, lighter than a full pressure set. Confirm the student can apply rules in real combined contexts — not overwhelm.

**Hard rules:**
- NO article-selection-only exercises
- Every exercise requires at least one active decision beyond gender recognition
- No word banks, no hints inside exercises
- Use lesson vocabulary where possible; max 1–2 new words per exercise
- Never repeat the same exercise type within the set
- Scale the number of exercises to lesson count:
  - 1–2 lessons → 3–4 exercises
  - 3–4 lessons → 5–6 exercises
  - 5+ lessons → 7 exercises

**Exercise types (never repeat type):**
- Sentence translation English → German, 8–12 items, each with one grammar decision point
- Sentence building from scrambled words (5–7 words each), 6–8 items
- Error detection in a short paragraph (8–12 errors, not labeled, student finds and rewrites)
- Fill-in-the-blank paragraph, NO word bank
- Sentence transformation (change gender / number / article type while keeping meaning)
- Short dialogue reconstruction — jumbled lines, student reorders AND applies grammar rules
- Mixed correction — 8–10 isolated sentences each with one error, student identifies and fixes

**Label each exercise with which lessons it targets:**
```
#### Exercise [N] — [type] *(Lessons: [X, Y])*
```

---

## Output Format

```markdown
# German Lesson Set — [topic range or Folge range]

---

## Part 1: Lesson Notes

### Lesson 1: [Title]
[clean notes]

### Lesson 2: [Title]
[clean notes]

...

---

## Part 2: Combined Practice Exercises

#### Exercise 1 — [type] *(Lessons: X, Y)*
[content]
⇒

#### Exercise 2 — [type] *(Lessons: X, Z)*
[content]
⇒

...

---

<details>
<summary>Answer Key</summary>

**Exercise 1**
1. ...

**Exercise 2**
...

</details>
```

---

## What NOT to Do

- Do not re-explain rules in your own words — restructure only
- Do not keep the teacher's original Übungen
- Do not use word banks
- Do not label traps inside exercises
- Do not exceed 7 exercises total regardless of lesson count
- Do not write any exercise that tests only one lesson in isolation
- Do not merge two lessons in Part 1 if they cover different grammar topics

---

## Input

Paste the raw PDF content below:

[PASTE HERE]
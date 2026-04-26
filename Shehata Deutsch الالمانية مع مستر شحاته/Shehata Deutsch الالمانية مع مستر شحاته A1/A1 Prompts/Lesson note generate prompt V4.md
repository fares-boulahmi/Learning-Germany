# Lesson Processor — German Grammar (A1→B1 Path)

## Your Job

You receive a raw copy-paste from a German grammar PDF. It may contain **multiple lessons** (anywhere from 1 to 7+). It may be messy: Arabic mixed in, broken formatting, repeated headers, OCR artifacts, duplicate exercises.

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

Process each detected lesson separately, in order. All lessons go into one Part 1, each under its own `###` heading.

**Rules:**

- Keep Arabic where it directly translates a grammar term or explains a concept. Remove Arabic that is filler, page notices, or copyright lines.
- Remove ALL of the teacher's original exercises (Übung 1, Übung 2, etc.).
- Remove page numbers, copyright notices, publisher warnings.
- Restructure into clean Markdown: `###` for lesson headers, `####` for subsections, tables for grammar paradigms, bullet points for rules, blockquotes for example sentences.
- Keep every grammar table — format as Markdown tables.
- Keep all example sentences, labeled under the rule they illustrate.
- Do NOT add explanations the teacher didn't give. Clean and restructure only.

---

## PART 2 — New Words

For **each lesson**, select a **maximum of 3 words** that appear in the lesson material and are the most grammatically useful for understanding the lesson content.

For each selected word:

1. State the word with its article and plural form (if a noun), or its infinitive and key conjugations (if a verb)
2. Write **2 sentences** in the **2 forms judged most useful** for that word given the lesson's grammar focus — chosen freely from: Nominativ, Akkusativ, Dativ, Singular, Plural, negation, or a case transformation. Label each sentence with the form used.

**Format per word:**

```
**[word]** ([article] / Plural: [...] — or — Verb: [infinitive], [er/sie form])
- ([Form 1]): [sentence]
- ([Form 2]): [sentence]
```

**Group under:**

```
### New Words — Lesson [N]: [Title]
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

## Part 2: New Words

### New Words — Lesson 1: [Title]
[max 3 words, 2 sentences each]

### New Words — Lesson 2: [Title]
[max 3 words, 2 sentences each]

...
```

---

## What NOT to Do

- Do not re-explain rules in your own words — restructure only
- Do not keep the teacher's original Übungen
- Do not merge two lessons in Part 1 if they cover different grammar topics

---

## Input

**PDF content:** [PASTE HERE]
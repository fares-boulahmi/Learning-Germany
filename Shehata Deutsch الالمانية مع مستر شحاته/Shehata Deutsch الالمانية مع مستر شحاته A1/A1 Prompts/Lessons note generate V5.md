Here's the edited prompt:

---

# Lesson Processor — German Grammar (A1→B1 Path)

## Your Job

You receive a raw copy-paste from a German grammar PDF. It may contain **multiple lessons** (anywhere from 1 to 7+). It may be messy: Arabic mixed in, broken formatting, repeated headers, OCR artifacts, duplicate exercises.

You will output **one clean Markdown file** with the lesson notes only.

---

## How to Detect Lesson Boundaries

A new lesson starts when you see any of:

- A new "Folge" or episode number (e.g. `Folge 36`, `Folge 37`)
- A new bold/uppercase title that introduces a new grammar topic
- A clear thematic break (e.g. Nominativ → Akkusativ → Dativ)

If boundaries are ambiguous, group by grammar topic, not by page.

---

## Clean Lesson Notes

Process each detected lesson separately, in order, each under its own `###` heading.

**Rules:**

- Keep Arabic where it directly translates a grammar term or explains a concept. Remove Arabic that is filler, page notices, or copyright lines.
- Remove ALL of the teacher's original exercises (Übung 1, Übung 2, etc.).
- Remove page numbers, copyright notices, publisher warnings.
- Restructure into clean Markdown: `###` for lesson headers, `####` for subsections, tables for grammar paradigms, bullet points for rules, blockquotes for example sentences.
- Keep every grammar table — format as Markdown tables.
- Keep all example sentences, labeled under the rule they illustrate.
- Do NOT add explanations the teacher didn't give. Clean and restructure only.

---

## Output Format

```markdown
# German Lesson Set — [topic range or Folge range]

---

### Lesson 1: [Title]
[clean notes]

### Lesson 2: [Title]
[clean notes]

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
# Generate German Practice Set [Number]

## Input Required

### 1. Error Report from Last Set
[PASTE CORRECTION REPORT HERE]

### 2. Lesson Summary (from Lesson Summarizer Prompt)
[PASTE COMPRESSED LESSON SUMMARY HERE]

---

## Your Task

Generate **TWO markdown files** that:
1. **Drill the student's active errors** (60% of content)
2. **Teach new content from lessons** (40% of content)

---

## FILE 1: "German Practice Set [X].md"

### Structure (8-10 sections total)

**PART A: Error Pattern Drills (60%)**

For each 🔴 **Critical** error from the report:
- One dedicated section with 12-15 targeted exercises
- Use lesson content as context when possible (e.g., if lesson teaches sentence structure AND student struggles with verb conjugation, combine both)

For each 🟡 **Medium** error:
- Integrate into mixed exercises (don't create separate sections unless error is severe)

**PART B: New Lesson Content (40%)**

For each lesson in the summary:
- One section testing the **Exercise Generation Priority #1** from that lesson
- Combine lessons that test the same concept
- Skip lessons that overlap with ✅ mastered patterns from error report

**PART C: Creative Application (2-4 tasks MAXIMUM)**

Choose exactly **2-4** from these options (never more):
- [ ] One formal dialogue (Sie register, 16-20 exchanges)
- [ ] One informal dialogue (du register, 16-20 exchanges)
- [ ] One mixed-register dialogue (du + Sie, 20-24 exchanges)
- [ ] One email/letter (formal OR informal, 12-16 sentences)
- [ ] One free paragraph (18-22 sentences, specific requirements)

**Each creative task MUST:**
- Test 5+ different grammar patterns (from errors + lessons)
- Include mandatory vocabulary from lessons
- Have explicit checklist of what to include
- Have explicit checklist of errors to avoid (from error report)

---

### Exercise Consolidation Rules

**MERGE these into single exercises:**
- Multiple translation sets testing same pattern → ONE translation section with 20-25 items
- Conjugation table + gap-fill conjugation → ONE exercise with table + contextual blanks
- Multiple fill-in-the-blank paragraphs → ONE longer paragraph with more blanks

**ELIMINATE these entirely:**
- Standalone conjugation tables (embed in context instead)
- Exercises testing ✅ mastered patterns from error report
- Exercises testing lesson content the student already knows (check error report)

**COMBINE these strategically:**
- If lesson teaches word order AND student struggles with verb conjugation, create exercises that test both simultaneously
- If lesson teaches new vocabulary AND student struggles with article gender, require articles in vocabulary exercises

---

### Formatting Requirements

**Section headers format:**
```
### Section [N]: [Error Pattern or Lesson Concept] — [Exercise Type]
⚠️ Targets: [List specific errors from report this section drills]
📚 Lesson Link: [Which lesson(s) this connects to]
```

**Exercise format:**
- Number all exercises clearly
- Use ⇒ for answer blanks
- Mark error traps with ![⚠️](data:image/gif;base64,R0lGODlhAQABAIAAAP///wAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw==) + error label
- Total set length: **2000-2500 words** (NOT 9000+)

---

## FILE 2: "Answer Key — Set [X].md"

Provide:
- Correct answers for every exercise
- Alternative acceptable answers where applicable
- Brief explanation of why common mistakes are wrong (reference error report)
- For creative tasks: model answer OR correction checklist

**Format:**
```
# Answer Key — Practice Set [X]

## Section [N]: [Name]

### Exercise [N.1]
1. [Answer] — [Brief note if needed]
2. [Answer]
[...]

### Exercise [N.2]
[Complete answer text or checklist]

---

## Creative Task Corrections

### Task 1: [Name]
**Model Answer:**
[Provide full correct version OR]

**Correction Checklist:**
- ✓ All [error pattern] instances correct?
- ✓ All [lesson structure] used properly?
- ✓ Vocabulary from lessons included?
```

---

## Quality Control

Before finalizing, verify:

**Efficiency:**
- [ ] No exercise type repeated more than twice
- [ ] All similar exercises merged into longer single exercises
- [ ] Creative tasks limited to 2-4 total (NOT 6-8)

**Targeting:**
- [ ] Every section explicitly states which error pattern or lesson it tests
- [ ] At least 60% of exercises target 🔴 Critical errors from report
- [ ] No exercises testing ✅ Mastered patterns

**Lesson Integration:**
- [ ] All "Exercise Generation Priorities" from lesson summary covered
- [ ] New vocabulary from lessons appears in exercises (not just isolated lists)
- [ ] Lesson grammar structures tested in context (not just explained)

**Length:**
- [ ] Total set: 2000-2500 words
- [ ] Each section: 200-350 words maximum
- [ ] Answer key: 1500-2000 words

---

## Example Section Structure

### ✅ GOOD — Consolidated and Targeted
```
### Section 3: Verb Position 2 + er/sie/es Conjugation Drill
⚠️ Targets: ERROR 3 (er/sie/es -t ending), L20 (verb position 2)
📚 Lesson Link: L20 Satzbau

Transform each sentence: Start with the time expression, then adjust verb position and conjugate correctly.

1. Er lernt jetzt Deutsch. → Jetzt _____ er Deutsch. ![⚠️](data:image/gif;base64,R0lGODlhAQABAIAAAP///wAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw==) (er conjugation + inversion)
2. Sie wohnt in Berlin. → In Berlin _____ sie. ![⚠️](data:image/gif;base64,R0lGODlhAQABAIAAAP///wAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw==) (sie conjugation + inversion)
[... 18 more similar items]
```

### ❌ BAD — Repetitive and Scattered
```
### Section 3: Verb Conjugation Table — sein
[Full conjugation table]

### Section 4: Verb Conjugation in Sentences — sein
[10 fill-in-the-blank sentences]

### Section 5: More Conjugation Practice — sein
[10 more fill-in-the-blank sentences]

### Section 6: Translate These Sentences — sein
[10 translation sentences]
```
(This should be ONE section with 20-25 items testing sein in various contexts)

---

## Output

Generate both files now based on the error report and lesson summary provided above.
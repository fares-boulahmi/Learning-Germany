
## Input Required
Paste your ** lessons** (in the format you provided) below:

[PASTE LESSONS HERE]

---

## Your Task

Analyze the lessons and extract a **concise summary** optimized for exercise generation.

For each lesson, provide:

### Lesson [Number]: [Title]

**Core Grammar Rules:**
- [Rule 1 in one sentence]
- [Rule 2 in one sentence]
- [Maximum 3-4 rules per lesson]

**Key Vocabulary Introduced:**
- [List only NEW words/phrases, max 15 items]
- [Format: German word/phrase — English meaning]

**Conjugation Patterns (if any):**
- [Verb type + endings, e.g., "Regular verbs: ich -e, du -st, er/sie/es -t"]
- [Only if lesson introduces NEW conjugation]

**Sentence Structures (if any):**
- [Pattern, e.g., "Position 1 → Verb → Subject → Rest"]
- [Only essential patterns]

**Common Traps:**
- [Student mistake examples from lesson practice, max 3]
- [E.g., "Confusing 'wo' (where-location) vs 'wohin' (where-to)"]

---

## Output Format

Deliver a **compact reference sheet** (500-800 words total for all  lessons) structured like this:
```
LESSONS [X-Y] SUMMARY FOR SET [Z]

═══════════════════════════════════════════════════════════

L20: Satzbau (1) — Sentence Structure
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
RULES:
- Aussagesatz: Verb ALWAYS position 2 (Subject → Verb → Rest OR Other → Verb → Subject → Rest)
- W-Frage: W-word → Verb → Subject → Rest

VOCABULARY: 
Aussagesatz (statement), W-Frage (W-question), Mittelfeld (middle field), unterstrichenen Satzteil (underlined sentence part)

SENTENCE PATTERNS:
- Normal: Ich lerne jetzt Deutsch
- Inverted: Jetzt lerne ich Deutsch (time expression first → verb → subject)

TRAPS:
- Verb not in position 2 when time/place starts sentence
- Forgetting subject-verb inversion after non-subject position 1

═══════════════════════════════════════════════════════════

L[XX]: [Next Lesson Title]
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
[Continue same format...]

═══════════════════════════════════════════════════════════

EXERCISE GENERATION PRIORITIES:
1. [Most important concept from these  lessons]
2. [Second most important]
3. [Third most important]

AVOID DRILLING (already mastered in previous sets):
- [List any concepts that appear in these lessons but are marked ✅ in the error report]
```

---

## Important Rules

**Brevity over completeness:**
- Skip example sentences unless they demonstrate a critical trap
- Skip exercises from the lessons (only extract rules/vocabulary)
- Combine similar rules into single bullet points

**Prioritize testable patterns:**
- Focus on structures that can be drilled (conjugations, word order, case)
- Minimize explanatory text

**Flag lesson overlaps:**
- If 2+ lessons cover the same grammar point, note: "L20-L22 all test [concept]"

**Link to error patterns:**
- If a lesson teaches something the student already struggles with (from error report), mark it: ⚠️ CONNECTS TO ACTIVE ERROR


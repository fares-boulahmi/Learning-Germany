You are a German language teacher. I will give you a list of German vocabulary words. For each word, generate all its meaningful real-world states depending on its type:

- **Verb** → conjugate in present tense for: ich, du, er/sie/es, wir, ihr, sie/Sie. Use a natural, logical sentence for each.
- **Noun** → show it in: Nominative singular, Accusative singular, Dative singular, Genitive singular, Nominative plural, Accusative plural, Dative plural. Use a natural sentence for each.
- **Adjective** → decline it with a noun in: Nominative (m/f/n), Accusative (m/f/n), Dative (m/f/n). Use a natural sentence for each.

Output the results as **two files**:

---

**File 1 – Markdown file** named `german_memo.md`
A single mixed table with these columns:

| German Sentence | English Translation | Arabic Translation  | Useful Info |

Rules for the **Useful Info** column:
- Keep it minimal but useful.
- Mention gender (m/f/n) only when helpful.
- Mention the case and reason if it adds value (e.g. "nach → always Dative").
- For verbs, mention the conjugation form (e.g. "ich-form", "ihr-form").
- Use short labels, no full sentences. Example: `Tisch (m) · Dative → dem` or `nach + Dative always`.
- If nothing useful to add, leave the cell empty.

---

**File 2 – CSV file** named `anki_german_arabic.csv`
- Anki-ready, semicolon `;` separator
- Two columns only: German sentence ; Arabic translation
- No header row
- Wrap each field in double quotes
- Arabic translation must be natural Arabic, not literal

---

Do not output anything outside the two files. Just create and return both files.

Here are my words:
[### Set 3: Shopping & Money

**Verbs:**

1. kaufen - to buy
2. verkaufen - to sell
3. bezahlen - to pay
4. kosten - to cost
5. sparen - to save
6. ausgeben - to spend
7. umtauschen - to exchange
8. zurückgeben - to return
9. bestellen - to order
10. liefern - to deliver
11. verdienen - to earn
12. leihen - to lend/borrow
13. schulden - to owe
14. überweisen - to transfer
15. abheben - to withdraw

**Nouns:**

1. der Preis - price
2. das Geld - money
3. der Euro - euro
4. die Rechnung - bill/invoice
5. die Quittung - receipt
6. das Bargeld - cash
7. die Kreditkarte - credit card
8. der Rabatt - discount
9. die Mehrwertsteuer - VAT
10. das Angebot - offer
11. der Einkauf - purchase
12. der Kunde - customer
13. die Kasse - cash register
14. das Konto - account
15. die Überweisung - bank transfer

**Adjectives:**

1. teuer - expensive
2. billig - cheap
3. günstig - affordable/favorable
4. kostenlos - free (of charge)
5. reduziert - reduced
6. ausverkauft - sold out
7. verfügbar - available
8. knapp - scarce
9. wertvoll - valuable
10. preiswert - good value]
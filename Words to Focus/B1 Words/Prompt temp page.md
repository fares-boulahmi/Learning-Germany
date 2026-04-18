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
[### Set 5: Travel & Transportation

**Verbs:**

1. reisen - to travel
2. fliegen - to fly
3. fahren - to drive/go
4. abfahren - to depart
5. ankommen - to arrive
6. umsteigen - to change (trains/buses)
7. buchen - to book
8. reservieren - to reserve
9. packen - to pack
10. übernachten - to stay overnight
11. besichtigen - to visit/sightseer
12. erkunden - to explore
13. verpassen - to miss
14. verzögern - to delay
15. erreichen - to reach

**Nouns:**

1. die Reise - trip/journey
2. der Urlaub - vacation
3. der Flughafen - airport
4. der Bahnhof - train station
5. die Haltestelle - stop
6. das Gleis - platform/track
7. der Zug - train
8. das Flugzeug - airplane
9. der Bus - bus
10. die Straßenbahn - tram
11. das Ticket - ticket
12. die Fahrkarte - ticket (train/bus)
13. der Koffer - suitcase
14. das Gepäck - luggage
15. der Ausflug - excursion

**Adjectives:**

1. direkt - direct
2. indirekt - indirect
3. rechtzeitig - on time
4. verspätet - delayed
5. gebucht - booked
6. verfügbar - available
7. ausgebucht - fully booked
8. einfach - single (ticket)
9. hin und zurück - return
10. bequem - comfortable
]
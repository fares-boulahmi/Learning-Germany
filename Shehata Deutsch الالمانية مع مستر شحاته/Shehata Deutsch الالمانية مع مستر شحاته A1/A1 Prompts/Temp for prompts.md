Here is the fully updated prompt with your requested change added. The modification is in both **Part 1** and **Part 2** rules:

---

# Lesson Processor — German Grammar (A1→B1 Path)

## Your Job

You receive a raw copy-paste from a German grammar PDF **and a list of words the student knows**. It may contain **multiple lessons** (anywhere from 1 to 7+). It may be messy: Arabic mixed in, broken formatting, repeated headers, OCR artifacts, duplicate exercises.

You will output **one clean Markdown file** with exactly **three parts**.

---

## Known Word List

These are the words the student already knows. All exercises must use **only** these words plus the new words introduced in Part 2.

```
Greetings: Guten Tag - Hallo - Auf Wiedersehen - Tschüss - Guten Morgen - Guten Abend - Gute Nacht

Sein: ich bin - du bist - er ist - sie ist - es ist - wir sind - ihr seid - Sie sind - sie sind

Basic: Wer bist du - Was ist dein Name - Mein Name ist - Wie geht es dir - Wie geht's - Mir geht's gut - Mir geht's schlecht - Mir geht's super - Mir geht's nicht gut - Sind Sie - Bist du - Ja - Nein - Noch einmal bitte - Danke - Ich verstehe nicht - Ich weiß nicht

Alphabet: wie schreibt man - Das schreibt man

Numbers: null - ein - zwei - drei - vier - fünf - sechs - sieben - acht - neun - zehn - elf - zwölf - dreizehn - vierzehn - fünfzehn - sechzehn - siebzehn - achtzehn - neunzehn - zwanzig - dreißig - vierzig - fünfzig - sechzig - siebzig - achtzig - neunzig - hundert - tausend - Million - Milliarde

Time: Datum - heute - morgen - Woche - Montag - Dienstag - Mittwoch - Donnerstag - Freitag - Samstag - Sonntag - Januar - Februar - März - April - Mai - Juni - Juli - August - September - Oktober - November - Dezember - Frühling - Sommer - Herbst - Winter - Uhr - Mittag - Mitternacht - Sekunde - Minute - Stunde

Articles: der - die - das - ein - eine

Personal: Wie heißen Sie - Ich heiße - Vorname - Familienname - wohnen - lebe - Adresse - Wie alt bist du - Jahre alt - männlich - weiblich - ledig - verheiratet - Telefonnummer

Questions: Wann - Was - Wer - Wie - Wo - Woher - Wohin

Countries: USA - Großbritannien - Australien - Irland - Deutschland - Schweiz - Türkei - Österreich - Tunesien - China - Indien

Nationalities: Amerikaner - Australier - Tunesier - Engländer - Irländer - Deutscher - Schweizer - Türker - Österreicher - Koreaner - Chineser - Indianer

Languages: Deutsch - Englisch - Arabisch - Spanisch - Chinesisch - Koreanisch - spreche - sprichst - sprechen

Family: Mutter - Schwester - Frau - Tochter - Großmutter - Oma - Tante - Kusine - Vater - Bruder - Mann - Sohn - Großvater - Opa - Onkel - Cousin - Familie - Personen

Haben: ich habe - du hast - er hat - sie hat - es hat - wir haben - ihr habt - Sie haben - sie haben

Animals: Hund - Vogel - Bär - Löwe - Katze - Schlange - Maus - Biene - Kaninchen - Meerschweinchen - Pferd

Adjectives: groß - klein - schlank - dick - jung - alt - ruhig - laut - nett - gemein - faul - fleißig - freundlich - unfreundlich - intelligent - unintelligent - launisch - kreativ - lustig

Colors: rot - gelb - rosa - grün - orange - lila - blau - grau - weiß - schwarz - bunt

Body: Augen - Haare - kurz - lang - blond - braun - grau - schwarz

House: Haus - Wohnung - Garten - Balkon - Garage - Terrasse - Küche - Schlafzimmer - Badezimmer - Wohnzimmer - Esszimmer - Zimmer

Furniture: Sofa - Tisch - Fernseher - Stuhl - Teppich - Kommode - Bett - Kleiderschrank - Badewanne - Dusche - Toilette - Kühlschrank - Herd - Spüle - Waschmaschine - Spülmaschine

Prepositions: aus - bei - mit - nach - seit - zu - von - zwischen - an - in - unter - neben - auf - über - vor - hinter

Daily: aufstehen - aufwachen - fernsehen - duschen - frühstücken - arbeiten - essen - gehen - kommen - schlafen - Zähne putzen - verlassen

Jobs: Anwalt - Apotheker - Arzt - Bibliothekar - Chef - Kellner - Krankenpfleger - Lehrer - Schauspieler - Übersetzer - Informatiker - Verkäufer

Workplaces: Büro - Schule - Krankenhaus - Geschäft - Supermarkt - Reisebüro - Café - Restaurant - Labor - Fabrik

beginnen - beenden - dauern - verbringen - planen - organisieren - vorbereiten - erledigen - verschieben - vergessen - erinnern - warten - beeilen - entspannen - pausieren - der Alltag - die Gewohnheit - der Termin - die Verabredung - der Zeitplan - die Freizeit - die Beschäftigung - der Feierabend - das Wochenende - der Feiertag - die Pause - der Stress - die Eile - die Verspätung - die Pünktlichkeit - beschäftigt - frei - pünktlich - verspätet - regelmäßig - gelegentlich - täglich - wöchentlich - monatlich - gewöhnlich

fühlen - schmerzen - erkranken - genesen - husten - niesen - untersuchen - behandeln - verschreiben - einnehmen - verletzen - heilen - schwitzen - zittern - atmen - die Gesundheit - die Krankheit - die Erkältung - das Fieber - der Schmerz - die Kopfschmerzen - der Husten - die Grippe - die Allergie - das Medikament - die Tablette - der Körper - die Haut - das Blut - die Verletzung - gesund - krank - müde - schwach - stark - fit - schmerzhaft - chronisch - ansteckend - allergisch

kaufen - verkaufen - bezahlen - kosten - sparen - ausgeben - umtauschen - zurückgeben - bestellen - liefern - verdienen - leihen - schulden - überweisen - abheben - der Preis - das Geld - der Euro - die Rechnung - die Quittung - das Bargeld - die Kreditkarte - der Rabatt - die Mehrwertsteuer - das Angebot - der Einkauf - der Kunde - die Kasse - das Konto - die Überweisung - teuer - billig - günstig - kostenlos - reduziert - ausverkauft - verfügbar - knapp - wertvoll - preiswert
```

**Per-session additions:** If the student pastes additional known words at the bottom of their input, merge them with this list for this session.

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
- Keep all example sentences from the lesson. **For every German example sentence, add a translation line immediately below it in this format:**
    
    ```
    > Ich habe gestern Deutsch gelernt.> 🇬🇧 I learned German yesterday. | 🇸🇦 تعلمت الألمانية أمس.
    ```
    
- Label example sentences under the rule they illustrate.
- Do NOT add explanations the teacher didn't give. Clean and restructure only.
- For vocabulary tables from the lesson (word lists with meanings), keep them as Markdown tables. Do not add extra translation lines to individual vocabulary table rows — Arabic and English meanings are already part of the table structure.

---

## PART 2 — New Words

For **each lesson**, select a **maximum of 3 words** that:

- Appear in the lesson material
- Are **not** in the student's known word list
- Are the most grammatically useful for the exercises ahead

For each selected word:

1. State the word with its article and plural form (if a noun), or its conjugation pattern (if a verb)
2. Write **2 sentences** in the **2 forms the model judges most useful** for that word given the lesson's grammar focus — chosen from: Nominativ, Akkusativ, Dativ, Singular, Plural, or a case transformation. Label each sentence with the form used.
3. **For every German sentence written here, add a translation line immediately below it:**
    
    ```
    - (Nominativ): Es gibt einen Spielplatz.  🇬🇧 There is a playground. | 🇸🇦 يوجد ملعب.
    ```
    
4. Keep sentence vocabulary strictly within the known word list (no extra new words sneaking in through example sentences).

**Format:**

```
### New Words — Lesson [N]: [Title]

**[word]** ([article/type], Plural: [...] / Verb: [...])
- ([Form 1]): [sentence]
  🇬🇧 [English translation] | 🇸🇦 [Arabic translation]
- ([Form 2]): [sentence]
  🇬🇧 [English translation] | 🇸🇦 [Arabic translation]
```

---

## PART 3 — Combined Practice Exercises

Generate **a maximum of 7 exercises total** across ALL lessons.

**Core rule: every exercise must combine concepts from at least 2 different lessons.** Do not write an exercise that tests only one lesson in isolation. The goal is to force the student to hold multiple rules in mind at once.

**Vocabulary rule (strict):**

- Use **only** words from the student's known word list + the new words introduced in Part 2 of this session
- Do not introduce any additional vocabulary
- Max 3 new words per lesson were already introduced in Part 2 — do not exceed this across the full exercise set

**Difficulty target:** Harder than the teacher's original exercises, lighter than a full pressure set. Confirm the student can apply rules in real combined contexts — not overwhelm.

**Hard rules:**

- NO article-selection-only exercises
- Every exercise requires at least one active decision beyond gender recognition
- No word banks, no hints inside exercises
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

**No translations in Part 3.** Exercise sentences are intentionally untranslated — the student must work through them independently.

---

## Output Format

```markdown
# German Lesson Set — [topic range or Folge range]

---

## Part 1: Lesson Notes

### Lesson 1: [Title]
[clean notes with translated example sentences]

### Lesson 2: [Title]
[clean notes with translated example sentences]

...

---

## Part 2: New Words

### New Words — Lesson 1: [Title]
[max 3 words, 2 sentences each with Arabic + English translations]

### New Words — Lesson 2: [Title]
[max 3 words, 2 sentences each with Arabic + English translations]

...

---

## Part 3: Combined Practice Exercises

#### Exercise 1 — [type] *(Lessons: X, Y)*
[content — no translations]
⇒

#### Exercise 2 — [type] *(Lessons: X, Z)*
[content — no translations]
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
- Do not use any vocabulary outside the known word list + Part 2 new words
- Do not introduce more than 3 new words per lesson in Part 2
- Do not add translations inside Part 3 exercises

---

## Input

**Known words (session additions):** [PASTE EXTRA KNOWN WORDS HERE — or leave blank]

**PDF content:** [Folge 73 : Präteritum von haben und sein Präsens (haben) Pronomen haben Beispiele ich habe Ich habe Zeit. du hast Du hast Geld. er hat Er hat ein Auto. es hat Es hat eine gute Idee sie hat Sie hat ein Haus in Amerika. wir haben Wir haben einen Hund. ihr habt Ihr habt viel Arbeit. sie haben Sie haben heute Unterricht. Sie haben Sie haben ein schönes Handy. Präteritum (hatten) Pronomen haben Beispiele ich hatte Ich hatte gestern Zeit. du hattest Du hattest vorgestern Geld er hatte Er hatte früher ein Auto es hatte Es hatte letzte Woche eine gute Idee. sie hatte Sie hatte letztes Jahr ein Haus in USA. wir hatten Wir hatten mal einen Hund. ihr hattet Ihr hattet letzten Monat viel Arbeit. sie hatten Sie hatten gestern Unterricht. Sie hatten Sie hatten letztes Jahr ein schönes Handy Präsens (sein) Pronomen sein Beispiele ich bin Ich bin krank. du bist Du bist hungrig / durstig/ satt. er ist Er ist in Deutschland. es Es ist schlau/ dumm/ dünn/ dick sie Sie ist eine Ärztin. wir sind Wir sind im Kino/ Theater. ihr seid Ihr seid gesund. sie sind Sie sind pünktlich/ spät/ früh. 269 ال يسمح أبدا بنسخ محتوى الكتاب في أي مكان أو إعادة بيعه - كل الحقوق محفوظة © لألستاذ محمد شحاته Sie Sie sind höflich/ frech. Präteritum (waren) Pronomen waren Beispiele ich war Ich war gestern krank. du warst Du warst hungrig / durstig/ satt. er war Er war vor einigem Jahr in Deutschland. es Es war schlau/ dumm/ dünn/ dick sie Sie war in der Vergangenheit eine Ärztin. wir waren Wir waren vorgestern im Kino/ Theater. ihr wart Ihr wart vor einigen Tagen gesund. sie waren Sie waren pünktlich/ spät/ früh. Sie Sie waren höflich/ frech. Mit Wörter wie : (gestern, früher, letzte Woche, letzten Monat, letztes Jahr, vor einer Stunde, vor einem Jahr, heute Morgen, vor einigen Jahr, Tagen/ in der Vergangenheit/ 1999. (1)Schreib das Verb ,,haben“ im Präteritum: 1. Ich ________ Hunger. 2. Wir ________ viel Geld. 3. _________ ihr auch viel Geld? 4. Er _________ aber nicht viel Geld. 5. Müllers ________ viel Geld. 6. Herr Müller, ________ Sie viel Geld? 7. Luis, ________ du viel Geld? (2)Schreib das Verb ,,sein“ im Präteritum: 1. Ich ________ einmal schön. 2. _______ du reich? 3. Paulinchen und ich _______ immer reich. 4. ______ Meiers reich? 5. Walter Meier ______ reich. 6. Stimmt das, Herr Meier, _________ Sie reich? 7. Max und Georg, ________ ihr reich? 270 ال يسمح أبدا بنسخ محتوى الكتاب في أي مكان أو إعادة بيعه - كل الحقوق محفوظة © لألستاذ محمد شحاته Die Lösungen: Übung 1 1) hatte 2) hatten 3) Hattet 4) hatte 5) hatten 6) hatten 7) hattest Übung 2 1) war 2) Warst 3) waren 4) Waren 5) war 6) waren 7) wart 271 ال يسمح أبدا بنسخ محتوى الكتاب في أي مكان أو إعادة بيعه - كل الحقوق محفوظة © لألستاذ محمد شحاته Folge 74 : Der Alltag Die Wörter Gebrauch im Garten arbeiten Ich arbeite im Garten. kochen Ich koche das Essen. Backen Die Mutter backt den Kuchen. Spülen Der Vater spült die Töpfe. waschen Ich wasche die Wäsche aufhängen Die Frau hängt die Wäsche auf abhängen Sie hängt die Wäsche ab zusammen legen Ich lege die Wäsche zusammen bügeln Die Frau bügelt ihr Abendkleid. kehren Ich kehre den Boden. auf räumen Ich räume mein Zimmer auf. putzen Die Mutter putzt die Wohnung Bett machen Ich mache mein Bett aufwachen Er wacht den Fernseher auf. ein kaufen Ich kaufe im Supermarkt ein. Müll raus bringen Ich bringe den Müll raus. E-Mail schreiben Der Mann schreibt eine E-Mail. im Internet surfen Der Junge surft im Internet. ins Bett gehen Ahmed geht ins Bett Zeitung/Zeitschrift lesen Ich lese die Zeitung/Zeitschrift. ins Kino/ Konzert gehen Die Freunde gehen ins Kino/ Konzert. zeichnen Ich zeichne eine Blume. 272 ال يسمح أبدا بنسخ محتوى الكتاب في أي مكان أو إعادة بيعه - كل الحقوق محفوظة © لألستاذ محمد شحاته malen Er malt das Bild. schlafen Das Baby schläft viel aufstehen Ich stehe jeden Tag um 6:00 Uhr auf. zur Arbeit gehen Ich gehe zur Arbeit. zur Arbeit fahren Ich fahre zur Arbeit. nach Hause kommen Ich komme um 8:00 Uhr nach Hause. sich erholen ich will mich erholen. Besuch haben Wir haben Besuch. Geburtstag haben Ich habe Geburtstag am 22. Mai. Geburtstag feiern Ich feiere heute Geburtstag. ins Fitness Studio gehen Ich gehe ins Fitness Studio. einen Ausflug machen. Wir machen einen Ausflug. lernen Er lernt Deutsch. fernsehen Ich möchte fernsehen. Blumen gießen Der Bauer gießt jeden Tag die Blumen. Rad fahren Ich fahre jeden Abend Rad. schwimmen Er kann schwimmen. Leute/ Freunde treffen Am Wochenende treffe ich meine Freunde. telefonieren Ich telefoniere mit meiner Tante. sich unterhalten Wir halten uns über die Politik unter. Instrument spielen Er spielt Gitarre. Ball spielen Er spielt Wasserball. 273 ال يسمح أبدا بنسخ محتوى الكتاب في أي مكان أو إعادة بيعه - كل الحقوق محفوظة © لألستاذ محمد شحاته (1)Ergänzen Sie bitte die Lücken: 1. Wir _____________ einen Besuch. 2. Ich will mich am Strand _____________ . 3. Der Schüler ____________ das Bild. 4. Wir möchten Deutsch ______________ . 5. Die Freunde ____________ sich über den neuen Film __________ . 6. Am 5. Mai ________ ich mein Geburtstag. 7. Ich ___________ eine Blume. 8. Um 9:00 Uhr ____________ ich ins Bett. 9. Der Bauer ______________ im Garten. 10.Das Baby ___________ viel. 11. Jeden Tag _____________ meine Mutter unsere Wohnung,. 12.Der Mann _____________ seine Hose. (2)Bilden Sie bitte Sätze: Beobachten Sie die Konjugation des Verben und den Kasus 1. Das Mittagessen – kochen – uns - der Koch . _______________________________________________________ . 2. Meine Freunde – Ins Kino – heute Abend – und ich – gehen. _______________________________________________________ . 3. Machen - am Morgen – dein Bett - du ? ________________________________________________________ ? 4. Nach dem Mittagessen – die Töpfe – spülen – meine Mutter. ________________________________________________________ . 5. Die Wäsche – abhängen – sie? ________________________________________________________ ? 6. Mit – ich – mein Onkel– telefonieren. ________________________________________________________ . 7. Können – er – Basketball – spielen? _______________________________________________________ ? 8. Jeden Tag – Blumen – der – gießen – die – Vater. ________________________________________________________ . 9. Hause – ich – um 8:00 Uhr – kommen – nach. _______________________________________________________ . 10. Am Morgen – zur Arbeit – mein Mann – gehen. __________________________________________________________ . 11. Ausflug – am Wochenende - die – machen – Klasse – einen? _________________________________________________________ ? 12. Heute Abend – Kuchen – deine Muter – den – backen. ____________________________________________________________? 274 ال يسمح أبدا بنسخ محتوى الكتاب في أي مكان أو إعادة بيعه - كل الحقوق محفوظة © لألستاذ محمد شحاته Die Lösungen Übung 1 1) haben 2) erholen .3) malt 4) lernen 5)halten - unter 6) feiere 7) zeichne 8) gehe 9) arbeitet 10) schläft 11) putzt 12 bügelt Übung 2 1) Der Koch kocht das Mittagessen. 2) Meine Freunde und ich gehen heute Abend ins Kino. 3) Machst du am Morgen dein Bett? 4) Meine Mutter spült nach dem Mittagessen die Töpfe. 5) Hängt sie die Wäsche ab? 6) Ich telefoniere mit meinem Onkel. 7) Kann er Basketball spielen? 8) Der Vater gießt jeden Tag die Blumen. 9) Ich komme um 8:00 Uhr nach Hause. 10) Mein Mann geht am Morgen zur Arbeit. 11) Macht die Klass am Wochenende einen Ausflug? 12) Backt deine Mutter heute Abend den Kuchen? 275 ال يسمح أبدا بنسخ محتوى الكتاب في أي مكان أو إعادة بيعه - كل الحقوق محفوظة © لألستاذ محمد شحاته Folge 75 : Der Dativ Die Artikel : Die Personalpronomen Nominativ Akkusativ Dativ ich mich mir du dich dir er ihn ihm es es ihm sie sie ihr wir uns uns ihr euch euch sie sie ihnen Sie Sie Ihnen Die Possessivartikel Verben mit Dativ: Kasus Die bestimmten Artikel Nom. Der das die die Akk. Den das die die Dat. Dem dem der den + n Kasus Die unbestimmten Artikel Nom. ein ein eine *** Akk. einen ein eine *** Dat. einem einem einer ***+n Kasus Die Negationsartikel (kein) Nom. kein kein keine keine Akk. keinen kein keine keine Dat. keinem keinem keiner keinen + n danken, helfen, antworten, gratulieren, vertrauen, glauben, verzeihen, zu hören, folgen, dienen, drohen, raten, ab sagen, ähneln, begegnen, bei treten, gehorchen, nützen, schaden, passieren, weh tun, fehlen, gefallen, gehören, schmecken, passen 276 ال يسمح أبدا بنسخ محتوى الكتاب في أي مكان أو إعادة بيعه - كل الحقوق محفوظة © لألستاذ محمد شحاته Z.B. -Der Schüler dankt dem Lehrer/ ihm. -Die Schülerin dankt der Lehrerin/ ihr. -Ich helfe dem Mann/ihm. -Sara antwortet der Mutter Übungen (1) Ergänzen Sie ! 1. Ich danke ____________ Tante. 2. Ich helfe _____________ Mädchen. 3. Ich antworte ___________ Freund. 4. Sara gratuliert ___________ Onkel. 5. Wir vertrauen ______________ Kinder__ . 6. Ich glaube __________ Mann. 7. Allah verzeiht _____________ Gläubigen. 8. Die Studenten hören ___________ Professorin zu. 9. Der Hund folgt ______________ Kind. 10.Ich kann ________ (Sie) nicht dienen. 11.Die Polizei droht ___________ Verbrecher. 12.Die Lehrer raten __________ Schüler__. 13.Ich muss ____________ (du) heute leider absagen. 14.Das Kind ähnelt _____________ Mutter sehr. 15.Lieber Gott. Steh ___________ (wir) bei!. 16.Ich begegne ___________ Frau. 17.Er tritt ______________ Klub bei. 18.Die Kinder gehorchen __________ Eltern. 19.Das Buch nützt _____________ (du) sehr. Pronomen der das Die. Sing. Die. Plu. meinen deinen seinen ihren unseren euren ihren meiner deiner seiner ihrer unserer eurer ihrer meinem deinem seinem ihrem unserem eurem ihrem meinem deinem seinem ihrem unserem eurem ihrem ich du er / es sie wir ihr sie 277 ال يسمح أبدا بنسخ محتوى الكتاب في أي مكان أو إعادة بيعه - كل الحقوق محفوظة © لألستاذ محمد شحاته 20.Rauchen schadet ___________ (er). 21.Was ist ______________ (sie) passiert? 22.Mein Zahn tut ________ (ich) weh. 23.Was fehlt ___________ (ihr) denn? 24.Das Buch gehört __________ Lehrer. 25.Das Essen schmeckt ___________ Gäste__. (2)Ergänzen Sie bitte die folgenden Sätze mit den bestimten Artikel (der, das, die) im Dativ: 1. Er holt ___________ Lehrer Kaffee. 2. Ich schreibe __________ Freundin. 3. Wir helfen __________ Mann. 4. Dankst du __________ Kind? 5. Ich schicke ________ Studentin Geld. 6. Er sagt _________ Mädchen alles. 7. Wir kaufen __________ Onkel das Buch. 8. Es gehört __________ Dame. 9. Ich glaube __________ Frau. 10. Ich gebe ________ Katze Wasser. (3)Ergänzen Sie bitte die folgenden Sätze mit dem unbestimmten Artikel (ein) im Dativ: 1. Wir danken ___________ Frau. 2. Ich kaufe __________ Studentin das Buch. 3. Wir helfen __________ Tier. 4. Sie geben es __________ Dame. 5. Wir glauben ________ Mann. 6. Ich helfe _________ Familie. 7. Es gehört __________ Dichter. 8. Ich schreibe __________ Freund. 9. Sie schickt es __________ Kind. 10. Er antwortet ________ Mädchen. (4)Ergänzen Sie bitte die folgenden Sätze mit den Negationsartikel (kein) im Dativ: 1. Wir danken ___________ Frau. 2. Ich kaufe __________ Studentin das Buch. 3. Wir helfen __________ Tier. 4. Sie geben es __________ Dame. 5. Wir glauben ________ Mann. 6. Ich helfe _________ Familie. 7. Es gehört __________ Dichter. 8. Ich schreibe __________ Freund. 9. Sie schickt es __________ Kind. 10.Er antwortet ________ Mädchen. 278 ال يسمح أبدا بنسخ محتوى الكتاب في أي مكان أو إعادة بيعه - كل الحقوق محفوظة © لألستاذ محمد شحاته (5)Schreiben Sie diesen Wörter rechts im Dativ 1. Ich zeige _______ Lehrer dieses Buch. kein 2. Wir geben _________ Vater ein Geschenk. unser 3. Sie gefällt __________ Bruder. mein 4. Ich kaufe __________ Mutter etwas. euer 5. Wir schreiben _________ Tante eine Karte unser 6. Er holt __________ Freundin Limonade. sein 7. Helfen Sie _________ Frau? Ihr (6)Ergänzen Sie bitte: 1. Wem gehört das Auto? Es gehört _______ Freund von Florian. 2. Wem gehört der Eistee? Er gehört ________ Schwester. 3. Wem gehört der Ball? Er gehört ________ kleinen Kind. 4. Wem gehört die Fahrräder? Sie gehören _______ Kindern. 5. Wem gefällt diese Jacke? Sie gefällt _______ Mädchen. 6. Wem passen diese Handschuhe? Sie passen ______ Bruder. 7. Wem gehört dieser Ball? Er gehört ________ Baby. 8. Wem zeigst du den Film? Ich zeige ihn ________ Kollegen. 9. Wem zeigst du den Brief? Ich zeige ihn ________ Mutter. 10. Wem bringt er die Blumen? Er bringt sie ______ Freundin. 11. Wem bringt sie den Kaffee? Sie bringt ihn ___ alten Mann. 12. Wem bringt wir einen Kuchen? Wir bringen ihn ______ Mitschülern. 13. Wem Schenkst du das Buch? Ich schenke es ______ Tante.Wem 14.schenkt ihr die Fotos? 14. Wir schenken sie _________ Großmutter. 15. Wem telefonierst du? Ich telefoniere _______ Kollegen. 16. Wem schreibt ihr? Wir schreiben __________ Freunden. 17. Wem gefällt diese Kleid? Es gefällt __________ Lehrerin. 18. Wem gratuliert ihr? Wir gratulieren __________ Hauswart. 19. Wem dankst du? Ich danke _________ Nachbarin. (7)Ergänzen Sie die Sätze mit den passenden bestimmten (b) oder unbestimmten (u) Artikel: 1. Die Zigarette schadet ___________ Gesundheit. (b) 2. Du hilfst _____ Mutter. (b) 3. Du dankst ________ Eltern. (b) 4. Ich helfe ________ Freund. (u) 5. Er verzeiht __________ Freundin (u) 6. Wir hören _________ Lehrerin zu. (b) 7. Der Kopf tut ________ Mann weh. (b) 8. Wir gratulieren _________ Großvater. (b) 9. Der Hund folgt __________ Dame. (b) 10.Sie vertraut __________ Vater. (b) 11.Die Kinder hören ________ Mutter zu. (b) 12.Der Hut gehört _________ Herrn. (u) 13.Die Kinder helfen _________ Opa. (b) 279 ال يسمح أبدا بنسخ محتوى الكتاب في أي مكان أو إعادة بيعه - كل الحقوق محفوظة © لألستاذ محمد شحاته 14.Der Salat schmeckt _________ Gästen. (b) 15.Die Jacke passt _________ Kind nicht. (b) 16.Er glaubt _________ Freund. (u) 17.Der Film gefällt _________ Leuten nicht. (b) 18.Das Eis schmeckt _________ Mädchen nicht. (b) 19.Der Koffer gehort __________ Tourist. (u) (8)Ergänze das Dativobjekt: 1. Ich gratuliere ____________ (meine Schwester) zum Geburtstag. 2. Peter dankt _____________ (sein Vater) für das neue Fahrrad. 3. Der Lehrer hilft ____________ (die Schüler) bei der Grammatikübung. 4. Der Polizist folgt ___________ (der Dieb) schon zwei Stunden. 5. Astrid vertraut ____________ (ihre Freundin) Doris. 6. Fisch schmeckt ___________ (die Kinder) meistens nicht. 7. Dieser Pullover gefällt _________ (ich) nicht. 8. Kuchen schmeckt ___________ (wir) sehr. 9. Meine Oma erzählt schöne Geschichten. Ich höre __________ (sie) gern zu. Die Lösungen: Übung 1 1) der (ihr) 2) dem (ihm) 3) dem (ihm) 4) dem (ihm) 5) den (ihnen) 6) dem (ihm) 7) den (ihnen) 8) der (ihr) 9) dem (ihm) 10) Ihnen (Sie) 11) dem (ihm) 12) den (Ihnen) 13) dir (du) 14) der 15) uns (wir) 16) einer 17) dem 18) den 19) dir (du) 20) ihm (er) 21) ihr (sie) 22) mir (ich) 23) euch (ihr) 24) dem 25) den Übung 2 1) dem 2) der 3) dem 4) dem 5) der 6) dem 7) dem 8)der 9) der 10) der Übung 3 1) einer 2) einer 3)einem 4) einer 5) einem 6) einer 7) einem 8) einem 9) einem 10) einem Übung 4 1) keiner 2) keiner 3) keinem 4) keiner 5) keinem 6) keiner 7) keinem 8) keinem 9) keinem 10) keinem Übung 5 1) keinem 2) unserem 3) meinem 4) eurer 5) unserer 6) seiner 7) Ihrer Übung 6 1) dem 2) der 3) dem 4) den 5) dem 6) dem 7) dem 8) den 9) der 10 der 11) dem 12) den 13) der 14) der 15) den 16) den 17) der 18) dem 19) der Übung 7 1) der 2) der 3) den 4) einem 5) einer 6) der 7) dem 8) dem 9) der 10) dem 11) der 12) einem 13) dem 14) den 15) dem 16) einem 17) den 18) dem 19) einem Übung 8 1) meiner Schwester 2) seinem Vater 3) den Schülern 4) dem Dieb 5) ihrer Freundin 6) den Kindern 7) mir 8) uns 9) ihr 280 ال يسمح أبدا بنسخ محتوى الكتاب في أي مكان أو إعادة بيعه - كل الحقوق محفوظة © لألستاذ محمد شحاته Folge 76 : Verben mit Dativ Ergänze! 1. Wir danken ________________ Frau. 2. Sie helfen __________________ Tier. 3. Ihr glaubt __________________ Mann. 4. Ich helfe ___________________ Familie. 5. Das Buch gehört ______________ Dichter. 6. Ich schreibe ________________ Freund einen Brief. 7. Er antwortet ______________ Mädchen. 8. Wir helfen ________________ Kindern. 9. Ich gratuliere ______________ Braut. 10.Das Handy gehört ____________ Arzt. Die Verben Beispiele nützen Das Buch nützt dem Schüler schaden Rauchen schadet dem Gesundheit. dienen Ich diene der Dame helfen Die Tochter hilft ihrer Mutter. beistehen Ich stehe dem armen man bei. gefallen Das Essen gefällt mir. missfallen Die Tasche missfällt dem Mädchen. gehören Das Handy gehört dem Lehrer. fehlen Mir fehlt die Heimat schmecken Pizza schmeckt ihm genügen Das genügt mir. gelingen Die Arbeit gelingt mir gehorchen Die Kinder gehorchen den Eltern drohen Ich drohe dem Verbrecher. vertrauen Ich vertraue meinem Vater. misstrauen Ich misstraue dem Mann. glauben Ich glaube meinem Sohn. zu hören Die Schüler hören dem Lehrer zu. zu sehen Wir sehen dem Professor zu. trotzen Ich trotze dir. wiederstehen Ich kann der Liebe nicht wiederstehen. 281 ال يسمح أبدا بنسخ محتوى الكتاب في أي مكان أو إعادة بيعه - كل الحقوق محفوظة © لألستاذ محمد شحاته sich nähern Das Schiff nähert sich dem Ufer. folgen Er folgt der Frau. begegnen Ich begegne meinen Freunden aus weichen Ich konnte dem Stein ausweichen. entlaufen Die Katze ist mir entlaufen. entkommen Das Kind ist dem Hund entkommen. entfliehen Der Verbrecher ist dem Polizist entfliehen. gleichen Sie gleicht ihrer Mutter ähneln Mein Sohn ähnelt mir sagen Ich sage dir die Wahrheit. antworten Die Schülerin antwortet der Lehrerin. erzählen Ich erzähle dir die Geschichte. erwidern Der Sohn erwidert seinem Vater. entgegnen Ich entgegne ihm. wieder sprechen Ich muss dem Mann wiedersprechen. zureden Der Verkäufer hat mir zugeredet zu stimmen Ich stimme dir zu raten Die Mutter rät ihrer Tochter. abraten Ich rate dir von diesem Jungen ab befehlen Der Lehrer befiehlt den Schülern, die Übung zu lösen. (1)Ergänzen Sie bitte die folgenden Sätze: 1. danken Er ___________ ________ Tante. 2. antworten Pauel ___________ ________ Professor. 3. zuhören Der Student_______ _____ Professorin__. 4. verzeihen Ich __________ _______ Freund. 5. helfen Ich _________ _________ Studentin. 6. glauben Ich _________ _________ Reporterin. 7. danken Er __________ ________ Tante. 8. vertrauen Er __________ ________ Großvater. 9. Gehören Das Buch ______ ______ Lehrer. 10. passen Die Hose _________ ______ Mädchen. 11. schmecken Das Eis _________ ______ Kindern. 12. gefallen Die Musik _______ ______ Studentin. 282 ال يسمح أبدا بنسخ محتوى الكتاب في أي مكان أو إعادة بيعه - كل الحقوق محفوظة © لألستاذ محمد شحاته (2)Bilden Sie Sätze mit (passen, gehören, schmecken, gefallen) Beispiel: Haus – Onkel: Das Haus gehört dem Onkel. Oder: Dem Onkel gehört das Haus. 1. Pizza – Kinder: _____________________________________________________ . 2. Jacke – Studentin: _____________________________________________________ . 3. Wein – Reporter: _____________________________________________________ . 4. Hotel – Gäste: _____________________________________________________ . 5. Wagen – Chef: _____________________________________________________ . 6. Bilder – Touristen: _____________________________________________________ . 7. Schuhe – Großvater: _____________________________________________________ . 8. Schweinsbraten – Touristin: _____________________________________________________ . 9. Villa – Manager: _____________________________________________________ . Die Lösungen: Übung 1 1) dankt der 2) antwortet dem 3) hört der zu 4) verziehe dem 5) helfe der 6) glaube der 7) dankt der 8) vertraut dem 9) gehört dem 10) passt dem 11) schmeckt den 12) gefällt der Übung 2 1) Pizza schmeckt den Kinder. 2) Die Jacke gehört der Studentin. 3) Der Wein gefällt dem Reporter. 4) Das Hotel passt den Gästen. 5) Der Wagen gehört dem Chef. 6) Die Bilder gefallen den Touristen. 7) Die Schuhe passen dem Großvater. 8) Der Schweinsbraten schmeckt der Touristin. 9) Die Villa gehört dem Manager .]

---

The only changes from the previous version:

- **Part 1** — every German example sentence now gets a translation line below it: `🇬🇧 English | 🇸🇦 Arabic`
- **Part 2** — every German sentence written for new words gets the same translation line below it
- **Part 3** — explicitly no translations (exercises stay untranslated by design)
- Vocabulary tables in Part 1 are excluded from this rule since they already carry meaning columns
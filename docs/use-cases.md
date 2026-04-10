# Use Cases & Ziele

## Projektbeschreibung

[Beschreibt hier in 2-3 Sätzen, welches Problem euer Chatbot löst und warum er gebraucht wird.]

## Zielgruppe

[Wer nutzt den Bot? Studieninteressierte? Aktuelle Studierende? Beides? In welcher Situation befinden sie sich?]

## Use Cases

#### Use Case 1: Studiengang-Informationen (Priorität: Hoch)
Hier geht es um allgemeine Fragen zum BSc Business AI. Das ist der wichtigste Use Case, weil er beide Zielgruppen betrifft.

Auslöser: Jemand überlegt, ob der Studiengang passt, oder will wissen, was man dort lernt.
Typische Fragen: „Was ist Business AI?", „Welche Berufsaussichten habe ich?", „Brauche ich Programmierkenntnisse?", „Was unterscheidet Business AI von Wirtschaftsinformatik?", „Ist das Studium auf Deutsch oder Englisch?"
Erwartetes Ergebnis: Der Bot gibt eine klare, kompakte Antwort und kann bei Bedarf auf die FHNW-Website verlinken.
Entities: study_program (Business AI, Wirtschaftsinformatik)
Intents: ask_study_info, ask_career_prospects, ask_requirements

#### Use Case 2: Modulinformationen (Priorität: Hoch)
Studierende und Interessierte wollen wissen, welche Module es gibt und was darin behandelt wird.

Auslöser: Jemand will wissen, was in einem bestimmten Semester oder Modul läuft.
Typische Fragen: „Welche Module gibt es im 3. Semester?", „Worum geht es im Modul Dialogsysteme?", „Wer unterrichtet Machine Learning?", „Wie viele ECTS hat das Modul NLP?"
Erwartetes Ergebnis: Der Bot nennt Modulname, Inhalt, Dozierende, ECTS – idealerweise aus einer Knowledge Base (z. B. Google Sheet mit Moduldaten).
Entities: module_name, semester (1–6), dozent
Intents: ask_module_info, ask_module_list, ask_dozent

##### Use Case 3: Fristen, Termine & Organisation (Priorität: Mittel)
Praktische Fragen rund um den Studienalltag.

Auslöser: Jemand will eine Frist nicht verpassen oder sucht organisatorische Infos.
Typische Fragen: „Bis wann muss ich mich für das Herbstsemester anmelden?", „Wann beginnt das Frühlingssemester?", „Wo ist der Campus?", „Wie erreiche ich die Studienberatung?"
Erwartetes Ergebnis: Der Bot nennt Datum/Frist oder Kontaktinfos. Bei veralteten Infos verweist er auf die offizielle Website.
Entities: semester_typ (FS/HS), jahr
Intents: ask_deadline, ask_semester_dates, ask_contact, ask_location

## Abgrenzung

[Was macht der Bot bewusst NICHT? Welche Anfragen werden an menschliche Berater:innen weitergeleitet?]

## Nutzerrecherche

[Wie erledigen Studierende diese Aufgaben heute? Welche Wörter und Phrasen verwenden sie?]

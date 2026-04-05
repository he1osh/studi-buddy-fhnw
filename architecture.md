# Architektur

## Informationsbedarf (Data Need)

[Welche Daten benötigt der Chatbot, um effektiv zu funktionieren?]

- **Datenquellen:** [z. B. FAQ-Dokument, Studienreglement, Modulbeschreibungen]
- **APIs:** [z. B. keine externen APIs / FHNW-API / ...]
- **Wissensdatenbank:** [z. B. Google Sheets mit Modulinfos, PDF-Dokumente]

## Konversationskanäle (Channel / UI)

[Über welche Kanäle ist der Bot verfügbar?]

- **Primärer Kanal:** [z. B. Web Chat auf der FHNW-Website]
- **Optionale Kanäle:** [z. B. Telegram, WhatsApp, MS Teams]
- **Begründung:** [Warum habt ihr diese Kanäle gewählt?]

## Framework

[Welches Conversational AI Framework verwendet ihr?]

- **Framework:** [z. B. Voiceflow / Botpress / RASA]
- **Begründung:** [Warum dieses Framework? Low-Code vs. Pro-Code? Verfügbare Features?]

## Bot-Architektur

### Übersicht

```
[Nutzer:in] → [Kanal: Web Chat] → [NLU] → [Dialogue Management] → [NLG] → [Antwort]
                                      ↕
                              [Knowledge Base]
                                      ↕
                              [Externe Aktionen]
```

### NLU (Natural Language Understanding)

**Intents:**

| Intent | Beschreibung | Beispiel-Trainingsphrasen |
|--------|-------------|--------------------------|
| [z. B. ask_module_info] | [Frage nach Modulinhalten] | ["Was lerne ich in Dialogsysteme?", "Welche Module gibt es?"] |
| [z. B. ask_deadline] | [Frage nach Fristen] | ["Bis wann kann ich mich anmelden?", "Wann ist Anmeldeschluss?"] |
| [z. B. ask_exam] | [Frage zur Prüfung] | ["Wie wird geprüft?", "Gibt es eine schriftliche Prüfung?"] |
| [z. B. greet] | [Begrüssung] | ["Hallo", "Hi", "Guten Tag"] |
| [z. B. goodbye] | [Verabschiedung] | ["Tschüss", "Danke, das war's"] |
| [z. B. fallback] | [Nicht verstanden] | — |

**Entities:**

| Entity | Typ | Beispielwerte |
|--------|-----|---------------|
| [z. B. module_name] | [Custom] | ["Dialogsysteme", "NLP Basics", "Machine Learning"] |
| [z. B. semester] | [Number] | [1, 2, 3, 4, 5, 6] |
| [z. B. study_program] | [Custom] | ["Business AI", "Wirtschaftsinformatik"] |

### Dialogue Management

[Wie verwaltet der Bot den Gesprächskontext? Zustandsbasiert, frame-basiert?]

### NLG (Natural Language Generation)

[Wie generiert der Bot Antworten? Template-basiert, KI-generiert?]

### Externe Aktionen / Integrationen

| Integration | Beschreibung | Technologie |
|-------------|-------------|-------------|
| [z. B. Knowledge Base] | [Modulinfos abrufen] | [z. B. Google Sheets via Make-Webhook] |
| [z. B. Feedback-Speicherung] | [Nutzerfeedback speichern] | [z. B. Make Data Store] |

## Ethische Aspekte

[Welche ethischen Überlegungen habt ihr berücksichtigt?]

- [z. B. Bot gibt sich klar als Bot zu erkennen]
- [z. B. Keine personenbezogenen Daten gespeichert]
- [z. B. Verweis an menschliche Beratung bei sensiblen Themen]

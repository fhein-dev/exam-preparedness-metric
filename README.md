# exam-preparedness-metric-builder

A single-page, blank exam-prep template. Enter your own exam's domains, questions, glossary and sets, then practice and track how ready you are. It works for most exam, since nothing is pre-filled.

## How it runs

The app is hosted locally on each device. There is no server, account or sign-in, and everything runs in the browser, so it also works without an internet connection. Your questions, glossary and progress are saved on that device only and are not shared or synced. To move to another device or keep a copy, use **Backup / new exam**.

## Features

**Build your exam**
- **Domains:** add your exam's domains with optional percent weights and a target score.
- **Questions:** enter them manually. Supported types are multiple choice, select all that apply, true/false, identification and fill in the blank. Typed answers are not case sensitive and can accept several answers separated by `;`. Each question can have an explanation.
- **Sets:** group questions into named sets. A quiz is also generated automatically for each domain, plus an "All questions" set.
- **Glossary:** add terms with a meaning, an optional scenario and a domain. Use **Bulk add** to paste many at once in the form `Term > meaning`, separated by new lines or commas.

**Practice**
- **Test mode:** answers are checked at the end and count toward your readiness metric.
- **Review mode:** the correct answer and explanation appear after each question, and nothing counts toward the metric.
- **Options:** choose the number of questions and an optional timer before each run.
- **Results:** you get a score, a per-domain breakdown, and missed questions grouped by domain. **Review missed with explanations** replays only the questions you got wrong in Review mode.
- **Flashcards:** filter by domain, search, and shuffle.

**Readiness metric**
- It uses your latest Test-mode answer to each question, weighted by domain weights (equal weights if none are set).
- A domain needs at least 5 answered questions to count.
- It shows a per-domain breakdown, your weakest domain, and coverage.
- Review-mode attempts and glossary match quizzes are not counted.

**Smart practice**
- **Spaced repetition:** questions answered in Test mode come back after 1 day if missed, then after 3, 7, 14 and 30 days as you keep getting them right. Flashcards work the same way using "Still learning" and "Knew it".
- **Practice my weakest domain:** starts a quiz from your lowest-scoring domain.
- **Glossary match quiz:** matches meanings to terms, built automatically from your glossary.

**Other**
- **Light and dark mode** toggle, with dark as the default. The layout works on phones.
- **Backup / new exam:** copy your data as text, paste it back to restore it, or start a blank exam for a different subject.
- **Data storage:** data lives in that device's browser (local storage), separate on every device. Back it up before clearing site data.

## Future plans

- **Simulated lab environment and performance-based questions.** Planned in stages: ordering and matching tasks, hotspot questions (click the problem on a diagram or log), a rule or table builder, and eventually a scripted command-line simulator. Tasks would be stored as data, with partial credit.
- **Lightweight local AI agent for generating questions.** Generation would run on the user's own machine, and questions would be imported through a file or paste. Imported questions would go into a review queue marked "AI-generated" and be approved before they count.
- **Bulk question import** in the same style as bulk glossary import, which the AI generator also needs.
- **Real-exam feel:** question navigator with flagging, crossing out options, keyboard shortcuts, a pass line and scaled score, a no-going-back option, and pacing hints.
- **Partial credit** for select-all-that-apply questions.
- **Better backups:** merge a backup into existing data instead of replacing it, plus backup reminders.
- **Accessibility:** adjustable text size and full keyboard navigation.

---

Made by https://github.com/fhein-dev

# Legal MCQ Lab — Expanded Course-Aligned Edition

This is a self-contained browser-based practice exam for the Introduction to Law workshops.

## What is included

- **312 questions** stored separately in `questions.js`.
- A readable/editable copy of the bank in `questions.csv`.
- A **20-random-question** practice mode.
- A randomized full-bank mode.
- Randomized answer positions.
- Saved progress in the browser.
- Flagging, question navigation, keyboard shortcuts, and end-of-session review.
- Explicit feedback explaining why a selected answer did not earn credit and identifying the correct course principle.
- A source/workshop label on every question.

## How to use it

1. Extract the ZIP file.
2. Keep `index.html` and `questions.js` in the same folder.
3. Open `index.html` in a modern browser.
4. Choose **Practice 20 random questions** or **Go through all 312 questions**.

No installation, server, account, or internet connection is required.

## How to share it

Share the complete ZIP file. Classmates should extract it before opening `index.html`; opening the HTML directly from inside a ZIP may prevent the question file from loading.

## Editing the question bank

The application reads `window.QUESTION_BANK` from `questions.js`. Each question has:

- `id`
- `topic`
- `stem`
- four `choices`
- `correct` answer index
- `explanation`
- `source`

The stored correct index is `0`; the app shuffles all answer positions when a session begins. If you add questions manually, use a unique ID and keep the correct answer as the first choice.

`questions.csv` is provided for review and proofreading. If it is edited, the equivalent change must also be made in `questions.js` before the app will use it.

## Important study note

The bank was checked against the uploaded Workshop 1–9 materials. It is a revision aid, not an official assessment or statement of law. Course staff may update slides, OSCOLA guidance, exam rules, or legal examples, so compare the bank against the newest official materials before distributing it.

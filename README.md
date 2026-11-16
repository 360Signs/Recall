# Recall — Revision Studio
A responsive, static flashcard app. Open `dist/index.html` or serve `dist` with any static web host. No build or paid services required.

## Features
- Subjects, editable colours and subcategories
- Question/answer, multiple choice, true/false and fill-in-the-blank cards
- Search, sorting, stars and subject/topic filters
- Flip-card sessions, written answers, mixed quizzes and generated multiple choice
- Immediate feedback, optional explanations, self-marking for equivalent written answers, missed-card practice
- Review streaks, mastery (3 correct in a row) and accuracy
- Browser-local automatic saving and validated JSON backup import/export

## Data
Cards and results are stored in localStorage on the current browser and origin. They do not sync automatically across devices or between hosting URLs. Export regularly; clearing browser data removes local cards. Sample cards are provided on first visit.

## GitHub Pages
Publish `dist` via the included GitHub Actions workflow. In repository Settings → Pages, select GitHub Actions. Alternatively copy the three files in `dist` to the repository root and publish main/root. The application uses relative asset paths and supports project Pages URLs.

## Validation
JavaScript syntax checked with `node --check dist/app.js`. Browser checks covered first load, card creation, reload persistence, filtering, written-answer normalization and quiz results.

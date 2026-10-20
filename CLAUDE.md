# Concept Lab: conventions for Claude

Interactive study pages, one self-contained HTML file per course (`index.html` = IS 465, `ds110.html` = DS 110). Hosted on Vercel as static files; no backend.

## Adding a course
- New course = new `<course>.html` on `main`, plus a tab in the `.courses` nav at the top of **every** page.
- Match the existing look: copy the `<style>` tokens and helpers from `ds110.html` (light + dark tokens, graph-paper background, Literata / Public Sans / JetBrains Mono).
- Each concept section: eyebrow with the exam question(s) it covers, a short lead, an interactive lab, "Remember" + "Common mistake" notes, two check questions, and a "Mark as understood" button. Progress is saved in `localStorage` (wrap every access in try/catch).
- Verify every code output and worked number by running it in real Python before committing.

## End-of-page review: always an Anki-style deck
The review questions at the end of a course page are a spaced review deck, **not a flat list**. Reuse the deck in `ds110.html` (section `#exam`, JS block "exam review deck"):
- One card at a time: question (+ code), a textarea to answer from memory, then **Show answer** reveals the model answer next to what was typed.
- Ratings: **Again** puts the card back 3 cards later, **Almost** 6 cards later, **Got it** removes it from the round.
- Output questions carry an exact answer (`x`) and show whether the typed answer matches.
- Status strip of all cards (current / coming back / got it), each linking to its concept section.
- Round summary lists the cards that needed more than one try, with **Practice the ones I missed** (new round with only those) and **Start all again**.
- Shuffled or exam-order toggle; restart asks for confirmation in the page (no `confirm()`); keyboard: Space shows the answer, 1 / 2 / 3 rate; state persists in `localStorage`.

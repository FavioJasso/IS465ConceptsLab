# Concept Lab

Interactive study pages for NJIT courses. Each course has its own tab at the top of the page.

## IS 465 · `index.html`

Advanced Information Systems, Lectures 4 and 5:

- **Part 1 · Inferential statistics**: sampling, the normal curve, the Central Limit Theorem, standard error, hypothesis testing, t-tests, Type I/II errors, choosing a test, a worked paired t-test, confidence intervals, and multiple-testing pitfalls.
- **Part 2 · Visualization**: Anscombe's quartet, marks and channels, choosing a chart from the question, honest axes, Simpson's paradox, and rules of thumb.

Content is based on lecture slides by Mark Cartwright (NJIT).

## DS 110 · `ds110.html`

Introduction to AI, midterm review. Thirteen concepts mapped to the 16 midterm questions:

- **Part 1 · Python**: classes and objects, global vs local namespaces (with a step-through of the exam's scope question), try/except, writing `count_odds`, `while True` / `break`, slicing, and string methods.
- **Part 2 · Regression**: deterministic vs probabilistic models, least squares (drag the line, then work it by hand), and the four steps of regression modeling.
- **Part 3 · AI concepts**: symbolic vs connectionist AI, the Turing Test and its limits, and weights and biases in a single neuron (tune it, then train it).
- **Practice**: an endless predict-the-output drill, a full exam review where you write each answer before revealing the model answer, and a printable one-page cheat sheet.

The code editor runs real Python in the browser with [Pyodide](https://pyodide.org), loaded on first use from jsDelivr.

## How each page works

Each concept has a short explanation, an interactive lab, a common mistake to avoid, and check questions. Progress, answers and drafts are saved in your browser only.

Each page is a single self-contained HTML file (plain HTML, CSS and JavaScript, no build step). Open it locally or host it with GitHub Pages.

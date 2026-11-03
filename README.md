# Concept Lab

Interactive study pages for NJIT courses. Each course has its own tab at the top of the page.

## IS 465 · `index.html`

Data Analytics for Information Systems, Lectures 4 to 7:

- **Part 1 · Inferential statistics** (Lecture 5): sampling, the normal curve, the Central Limit Theorem, standard error, hypothesis testing, t-tests, Type I/II errors, choosing a test, a worked paired t-test, confidence intervals, and multiple-testing pitfalls.
- **Part 2 · Visualization** (Lecture 4): Anscombe's quartet, marks and channels, choosing a chart from the question, honest axes, Simpson's paradox, and rules of thumb.
- **Part 3 · Data management** (Lecture 6): primary and foreign keys (find the key in the poll table), relational algebra on the Books table with SQL and pandas side by side, the three anomalies and normalization, joins (including the orphan-row poll), OLTP vs OLAP and row vs column storage, fact and dimension tables and grain, star vs snowflake vs one big table, an OLAP cube you can slice, dice, drill, roll up and pivot, and ETL/ELT with an OData URL builder.
- **Part 4 · Data structures and algorithms** (Lecture 7): linear vs binary search (step through both), sort once / search many with the break-even k, Big-O growth and a drop-the-constants drill, arrays vs linked lists, a toy hash table with collisions, stacks and queues, binary search trees and balance, a BFS/DFS stepper on the lecture's practice graph and tree, and choosing a structure.
- **Practice**: two check questions per concept, and a review deck for Lectures 6 and 7 (write your answer, reveal, rate yourself; cards you miss come back a few cards later, and you can drill only the ones you missed).

Content is based on lecture slides by Mark Cartwright (NJIT).

## DS 110 · `ds110.html`

Introduction to AI, midterm review. Thirteen concepts mapped to the 16 midterm questions, plus thirteen from the lecture slides:

- **Part 1 · Python**: classes and objects, global vs local namespaces (with a step-through of the exam's scope question), try/except, writing `count_odds`, `while True` / `break`, slicing, and string methods.
- **Part 2 · Regression**: deterministic vs probabilistic models, least squares (drag the line, then work it by hand), and the four steps of regression modeling.
- **Part 3 · AI concepts**: symbolic vs connectionist AI, the Turing Test and its limits, and weights and biases in a single neuron (tune it, then train it).
- **Part 4 · Lecture slides**: thirteen more concepts from the course lectures that the midterm review doesn't cover: what counts as AI and GOFAI vs ML, the ML workflow and datasets, decision trees and overfitting, the confusion matrix, training a neural network (backprop, gradient descent), least squares by the table method, images and color spaces, filtering and convolution, CNN building blocks, ImageNet/AlexNet/VGG, self-supervised speech learning, ethics and bias, and fairness trade-offs.
- **Practice**: an endless predict-the-output drill, a review deck of all 16 exam questions (write your answer, reveal, rate yourself; cards you miss come back a few cards later, and you can drill only the ones you missed), a second review deck for the Part 4 lecture topics, and a printable one-page cheat sheet.

The code editor runs real Python in the browser with [Pyodide](https://pyodide.org), loaded on first use from jsDelivr.

## How each page works

Each concept has a short explanation, an interactive lab, a common mistake to avoid, and check questions. Progress, answers and drafts are saved in your browser only.

Each page is a single self-contained HTML file (plain HTML, CSS and JavaScript, no build step). Open it locally, or deploy the repo as a static site (it is hosted on Vercel); no server is needed.

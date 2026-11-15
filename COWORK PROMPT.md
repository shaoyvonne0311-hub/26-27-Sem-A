# Prompt for Claude Cowork (paste everything below the line)

---

You are helping me (a CityU student) set up my FINAL-EXAM revision system inside my Obsidian vault. You can read and edit files on my Mac. Work carefully and tell me what you changed.

## 0. Safety rules (follow strictly)
1. **Back up first.** Before changing anything, copy my whole GE1359 vault and my main `Dashboard.md` to a dated folder in a normal location (Documents, NOT a temp folder: macOS temp cleanup nearly destroyed my vault before). Tell me the backup path.
2. Never delete or overwrite existing GE1359 midterm files. Add new files; edit existing files only where stated, and show me the diff summary.
3. Ask me before any bulk rename/move. Do not touch anything outside the vault and the course folders I name.

## 1. Context
- Exams: CB2203 Thu 10 Dec 09:30 (50%) - GE1359 Sat 12 Dec 18:30 (70%) - CB2240 Mon 14 Dec 14:00 (40%) - MKT3601 Tue 15 Dec 09:30 (40%, open book) - MKT3603 Wed 16 Dec 14:00 (50%, A4 cheat sheet).
- My existing vault `GE1359 Revision Vault` has this structure: `00 Start Here`, `01 Plan` (Calendar, Daily), `02 Guides` (Question-Type Playbook, Memorise Sheet, Revision Guide, Past Paper Analysis), `03 Tracker` (Excel G/Y/O/R tracker, "RRT" layout, 17 question types x dates), `04 Tests`, `05 Practice Packs`, `06 Mind Maps` (Canvas), `07 Mistakes` (Mistake Log), `08 Flashcards` (Spaced Repetition plugin `question :: answer`, tags `#flashcards/<course>/<topic>`), `09 Source PDFs`. My main `Dashboard.md` is a dataviewjs page (css class `dashboard`, container class `db-home`) with a "GE1359" column.
- Claude (in chat) has already generated a ready-made folder called **`Finals 2026 Vault`** (I will put it on my Mac next to my vault; its path is: `<I will tell you>`). It contains: `00 Start Here.md`, `01 Plan/` (`Calendar.md`, `Time Budget.md`, `plan.json`, `Daily/` with 41 daily notes 2026-11-06 to 2026-12-16), and one `00 Course Hub.md` per course folder.
- `plan.json` is the single source of truth for the schedule (days -> tasks -> course, hours, title).

## 2. Tasks (in order)
**A. Import.** Move/copy `Finals 2026 Vault` into my Obsidian vault as a top-level folder `Finals 2026` (keep GE1359 Revision Vault untouched). Make sure all `[[wikilinks]]` resolve (Calendar, Time Budget, Start Here, daily notes, course hubs). Fix any broken link.

**B. Course skeletons.** For each of MKT3601, MKT3603, CB2203, CB2240 and GE1359 Final, inside its course folder create the same sub-structure as my GE1359 midterm vault: `01 Plan` (link to the shared plan), `02 Guides` (Question-Type Playbook, Memorise Sheet or Concept Glossary, Revision Guide), `03 Tracker`, `04 Tests`, `05 Practice Packs`, `06 Mind Maps`, `07 Mistakes/Mistake Log.md`, `08 Flashcards/<course> Flashcards.md` (with the Spaced Repetition how-to header), `09 Source PDFs`. For GE1359 Final, link to (do not copy) the existing Playbook, Mistake Log and Memorise Sheet and add a "Final additions" note for Ch4 and Ch5.

**C. Source PDFs.** Copy my course materials from my local course folders (I will tell you where) into each `09 Source PDFs`: MKT3601 China Business Environment, MKT3603 Consumer Behaviour (Lectures 1-9), CB2203 Data-driven Business Modeling (Lectures, Tutorials, Course Outline), CB2240 Intro to Bus Prog in Python (ppt, quiz, quiz last sem, classwork, homework, syllabus), GE1359 Algebra. Do not edit the PDFs. List anything that is missing.

**D. Trackers.** For each course create `03 Tracker/<course> Tracker.xlsx` by copying the layout and colour rules of `GE1359 Revision Tracker.xlsx` (rows = topics, columns = dates Nov 6 - Dec 16, cells G/Y/O/R with the same conditional formatting, "P" = planned revisit). Use these rows:
- MKT3601: Culture Map (8 dimensions); regional differences + tier cities; hukou/aging/urbanisation; Five Year Plan; SOE reform; agricultural reform; non-state sector + opening-up; FTZ names + definitions; Rostow, regional disparity, BRI, trade war; entry modes (pros/cons); marketing mix + standardisation vs adaptation; STP + segmentation; e-commerce trends; sustainable development; timed essays.
- MKT3603: one row per lecture topic (Motivation, Attention & Perception, Learning & Memory, Attitudes & Persuasion, Decision-Making, Shopping & Buying, Post-purchase, Self & Identity, Social Influence, Culture) + MCQ mocks + cheat sheet.
- CB2203: LP formulation/Solver, sensitivity analysis, IP, NLP, simulation (Monte Carlo/newsvendor/queueing/overbooking), regression/ANOVA, Excel-input fill-ins, MCQ output reading.
- CB2240: variables/expressions/strings, lists/tuples, conditionals, loops, functions, data handling, code tracing/debugging, code writing, cheat sheet.
- GE1359 Final: reuse the 17 midterm types + Ch3 remainder, Ch4 induction, Ch5 binomial, Ch5 combinatorics.
Pre-fill "P" cells on the days when `plan.json` schedules that course.

**E. Dashboard.** Edit my main `Dashboard.md` (after the backup): add a new column "🎓 Finals" that follows the existing dataviewjs style and does NOT break the GE1359 column. It should show: (1) countdown cards for the 5 exams (days left, date/time); (2) today's tasks read from `Finals 2026/01 Plan/Daily/<today>.md` (course, hours, title) with a click-to-open link; (3) hours planned vs hours done per course (done = ticked tasks in the daily notes); (4) a "next exam" banner. If dataview is unavailable, use plain markdown tables and tell me.

**F. Mind maps.** For each course create a `Scope Map.canvas` in `06 Mind Maps` (nodes = the tracker rows above, grouped by chapter/week; star the topics marked ★ in the MKT3601 hub).

**G. Verify and report.** Open each new note to check frontmatter is valid and links work, check the dashboard renders, then give me a short list: files created, files modified, anything skipped or uncertain, and anything I must do by hand.

## 3. Style
English notes, concise. Keep my existing emoji/callout style (`> [!abstract]`, `> [!warning]`). Keep file names exactly as given. If something is unclear, ask me one short question instead of guessing.

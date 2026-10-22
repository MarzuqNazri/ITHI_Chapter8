[README.md](https://github.com/user-attachments/files/33797337/README.md)
# Tourism Experience Control Centre — DHM1023 Chapter 8

A bilingual (English/Bahasa Malaysia), browser-based learning game for **Diploma in Hotel Management** and **Diploma in Event Management** students studying **Introduction to Hospitality and Tourism Industry (DHM1023), Chapter 8: Recreation, Attractions, Festivals & Events, and Gaming Entertainment**.

## Files
- `index.html` — page structure and screens
- `style.css` — responsive styling and visual design
- `script.js` — game logic and editable bilingual question bank

## Run locally
1. Download and extract the ZIP.
2. Open `index.html` in a modern browser. No server, build step, account or backend is required.
3. Internet is only needed for the optional Google Fonts import; system fallback fonts are defined.

## Publish on GitHub Pages
1. Create or open a GitHub repository.
2. Upload `index.html`, `style.css`, `script.js`, and `README.md` to the repository root.
3. Go to **Settings → Pages**.
4. Under build/deployment, choose **Deploy from a branch**, select the branch (usually `main`) and `/ (root)`, then save.
5. Open the published URL after deployment completes.

## Learning design
- 10 progressive stations; later stations remain locked until the current challenge is answered correctly.
- English and Bahasa Malaysia prompts and options.
- Students cannot advance after an incorrect answer; they must retry until correct.
- On a correct answer, the game explains the concept and displays a specific connection to the Chapter 8 slide content before the student continues.
- Scoring: 10 points for a correct answer on the first attempt; 5 points if the student needed one or more retries. Each question awards points only once, for a maximum of 100 points.
- Progress indicator, result report and review section.
- No countdown timer; approximately 15 minutes is a suggested classroom target.
- Keyboard, mouse and touch-friendly controls; responsive layout.

## Edit the question bank
Open `script.js` and edit the `questions` array at the top. Each question object contains:
- `zone`, `icon`, `scene`: station display labels
- `en`, `ms`: question in English and Bahasa Malaysia
- `options`: array of `[English option, Bahasa Malaysia option]` pairs
- `answer`: zero-indexed correct option (0 is A, 1 is B, 2 is C, 3 is D)
- `ex`, `exms`: answer explanations in English and Bahasa Malaysia

If changing the number of questions, also review references to the number `10` in the interface and result logic.

## Source alignment
Content is based on the supplied `Table 4 IHTI.pdf` and `Chapter 8 - Recreation Attractions Festivals and Events and Gaming Entertainment.pdf`. The Table 4 course learning outcomes include describing hospitality/tourism sectors and their characteristics, presenting findings from an organisational study, and discussing current sector trends. Chapter 8 concepts assessed include recreation/leisure/wellness, provider categories, attraction categories, event classification, destination impacts, event operations, integrated casino resorts, wellness trends and responsible management.

## Manual test checklist before classroom use
- [ ] Start button and instructions navigation
- [ ] Selecting and submitting an answer
- [ ] Incorrect answer shows feedback and permits retry
- [ ] Correct answer unlocks next station
- [ ] Score, progress and first-attempt count update correctly
- [ ] Completion report and concept review
- [ ] Restart resets progress
- [ ] Home navigation confirmation works
- [ ] Test desktop and mobile viewport sizes

The project is a static prototype. Test it in the target browser before using it with students.

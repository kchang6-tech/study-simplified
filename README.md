# Study Simplified

Study Simplified is a prototype that demonstrates how college students could turn confusing lecture notes into easier-to-understand study materials.

## First Working Slice

The prototype allows a user to:

1. Paste lecture notes into a text box.
2. Click "Simplify My Notes." 
3. View a study guide containing an explanation, 3 key concepts, and 3 practice questions.

The prototype also provides feedback when the user submits an empty or unclear input.

## How to run

Local (quick):

1. Clone the repository or download the files.
2. Open `index.html` in any modern browser (double-click the file). No server or account required.

Replit (recommended for an easy shareable link):

1. Open: https://replit.com/github/kchang6-tech/study-simplified
2. Click "Import from GitHub" (Replit will create a static web Repl). 
3. Click **Run** and use the Preview pane to interact with the prototype.

Note: I cannot create the Replit project for you from here, but the import link above will let you create one in a few clicks.

## Main features / validation

- Title and subtitle are shown prominently.
- Large textarea with placeholder: "Paste your lecture notes here..."
- Button: "Simplify My Notes" that updates results without a page refresh.
- Validation: If the textarea is empty, a helpful error message appears.
- Short or unclear inputs trigger a clear warning that the result may not be useful.
- A transparency notice is present: "Prototype demo: study guides use prepared sample responses. Live AI analysis is not connected yet."

## Quick test results (honest)

| Test                  | Input or Action                                              | What Happened                                                                                         | Result  |
| --------------------- | ------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------- | ------- |
| Typical case          | Submitted notes about revenue, expenses, and profit.         | The app matched the input to the Income Statement sample and displayed an explanation, concepts, and questions. | Pass    |
| Challenge case        | Submitted a focused question about taxes and revenue (not directly covered). | The app matched using keyword fallbacks ("revenue") and returned a related sample; the response was not tailored to taxes. | Partial |
| Invalid / empty case  | Submitted an empty text box and clicked the button.          | The app showed a clear error message asking the user to paste their notes first and did not produce a study guide. | Pass    |

## Files in this repository

- `index.html` — The complete single-file prototype (HTML, CSS, JS).
- `README.md` — This document.

## Known limitations (documented)

1. Simulated AI: The prototype uses prepared sample responses and simple keyword matching rather than live AI, so it cannot reliably analyze arbitrary course material.
2. Limited subject coverage: Examples focus on basic business and finance topics; many subjects are not covered.
3. Not validated for accuracy: The generated study guides are illustrative and have not been reviewed or tested for correctness by instructors.

## Future improvements

- Connect the prototype to a live AI backend to analyze arbitrary notes.
- Add more prepared samples and improve the matching logic.
- Add export/print and user-editable adjustments to the study guide.

## Links

- GitHub repository: https://github.com/kchang6-tech/study-simplified
- Replit import link (create a Repl from this repo): https://replit.com/github/kchang6-tech/study-simplified

---

If you'd like, I can also:

- Add a LICENSE (MIT) to the repo.
- Create a small GitHub Pages workflow to host `index.html` from the `main` branch so you have a live URL (this would add a simple GitHub Action). 

Which of those would you like me to do next?
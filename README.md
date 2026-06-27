# Flashcards

A small collection of mobile-friendly flashcard web apps for technical study. Swipe-based, runs entirely in the browser, no backend. A landing page ties the decks together.

**Decks (401 cards total):**

- **Machine Learning & Data Science** — 167 cards, 14 sections
- **ML & Data Engineering** — 120 cards, 14 sections
- **SQL** — 114 cards, 13 sections

## Features

- **Tap to flip** — front shows the concept, back shows "What it is" + an example (reference cards show a quick-reference table).
- **Swipe to study** — swipe right (or ✓) = got it, swipe left (or ✗) = review later.
- **Review / Known / New trays** — filter to just the pile you want to study.
- **Search** — jump to any card by number, or search by keyword (matches are highlighted).
- **Undo** — reverse the last swipe.
- **Resume** — reopens where you left off; progress is saved per deck in the browser (localStorage), no login or server.
- Works on phone and desktop; keyboard shortcuts on desktop (← review, → got it, space flip, Z undo).

## Project structure

```
index.html          landing page (lists every deck)
ml-ds.html          Machine Learning & Data Science
mle-de.html         ML & Data Engineering
sql.html            SQL
build.py            generator: PPTX → deck HTML + landing page
deck_template.html  shared design used for every deck
*.pptx              source PowerPoint decks (input for build.py)
ADDING_DECKS.md     how to add or hand-write new decks
```

The four HTML files are what gets served. `build.py`, `deck_template.html`, and the `.pptx` sources are kept so any deck can be regenerated or restyled.

## Run locally

Open `index.html` in any browser, or open a deck file directly. Everything is self-contained.

## Rebuild from PowerPoint

```bash
pip install python-pptx
python3 build.py
```

Regenerates every deck listed in `build.py` plus `index.html`. See **ADDING_DECKS.md** for adding a new deck.

## Deploy free on GitHub Pages

1. Create a free **public** repo on [github.com](https://github.com).
2. Upload the project files (drag them into **Add file → Upload files**, then commit).
3. **Settings → Pages → Deploy from a branch → `main` / root → Save.**
4. After ~1 minute your site is live at `https://<your-username>.github.io/<repo>/`.

Share that link — it opens the landing page, and every deck works on any phone.

## Cost

Free. GitHub Pages is free for public repositories.

## License

MIT — see `LICENSE`.

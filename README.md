# ML & DS Flashcards

A mobile-friendly flashcard web app for learning Machine Learning & Data Science concepts. Tinder-style swipe UX, runs entirely in the browser, no backend.

**167 cards** — 145 numbered concept cards across 14 sections, plus 22 hyperparameter & metric reference cards.

## Features

- **Tap to flip** — front shows the concept, back shows "What it is" + an example.
- **Swipe to study** — swipe right (or ✓) = got it, swipe left (or ✗) = review later.
- **Progress saved** — your known cards persist in the browser (localStorage); no login, no server.
- **Search by number** — jump straight to any card by its number.
- **Section filter** — focus on one topic (Neural Networks, NLP, Econometrics, etc.).
- **Shuffle** and keyboard shortcuts (← review, → got it, space to flip) for desktop.

## Run it locally

Just open `index.html` in any browser (Chrome or Safari on phone, or desktop). That's it — everything is in one file.

## Deploy free on GitHub Pages

1. Create a free account at [github.com](https://github.com).
2. Click **New repository**, name it (e.g. `ml-flashcards`), set it **Public**, click **Create**.
3. On the repo page, click **Add file → Upload files**, drag in this `index.html`, and **Commit**.
4. Go to **Settings → Pages**, under *Source* pick **Deploy from a branch**, choose `main` / `root`, **Save**.
5. Wait ~1 minute. Your link appears at the top of the Pages settings: `https://<your-username>.github.io/ml-flashcards/`

Share that link — it works on any phone.

> Note: the file must be named **`index.html`** for GitHub Pages to serve it automatically.

## Cost

Free. GitHub Pages is free for public repositories.

# A letter for you

A single-page static site. No build step, no dependencies. It works on GitHub Pages as is.

## Files

- `index.html` the page (letter, short version, reply box)
- `config.js` your name, their name, and an optional chat link
- `README.md` this file

## Put it on GitHub Pages

1. Create a new repository on GitHub. Pick a neutral name, since it becomes part of the link.
2. Upload `index.html` and `config.js` to the repository root (Add file > Upload files), then commit.
3. Go to Settings > Pages. Under "Build and deployment", choose "Deploy from a branch", pick the `main` branch and the `/ (root)` folder, then save.
4. After a minute or two the site is live at `https://YOUR-USERNAME.github.io/REPO-NAME/`.

To address it to them by name without editing any file, share a link like `https://YOUR-USERNAME.github.io/REPO-NAME/?to=Sam`.

## Preview on your computer

Open `index.html` in a browser, or run `python3 -m http.server` in this folder and visit `http://localhost:8000`.

## Customize

- Edit `config.js` to set `name`, `from`, and `contactUrl`.
- The letter text lives in `index.html` inside `<article>`. Edit the paragraphs directly.
- The reply buttons never send anything. They fill a message box that the reader can copy, or open your chat link if you set `contactUrl`.

## Privacy notes

- GitHub Pages sites are public. Anyone with the link can read the page, and the repository files are visible if the repository is public. Keep personal details like your full name, phone number, and address out of the text and out of `config.js`.
- The page asks search engines not to index it (`noindex`), but that is a request, not a lock.
- The fonts load from Google Fonts. If they are blocked, the page falls back to system fonts.

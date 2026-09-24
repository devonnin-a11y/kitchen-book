# Kitchen Book

**Professional Recipe Encyclopedia + Full Holistic System**

A clean, offline-capable, GitHub-ready recipe and natural remedies library.

## Features

- **120+ curated recipes** across Italian, French, Chinese, Japanese, Thai, Korean, Indian, Mexican, Mediterranean, American, and World cuisines
- **Home** and **Professional** cooking styles
- **Ingredient matching** — select what you have, get ranked recipes
- **Full Holistic section** — Hair, Skin, Digestion, Immunity, Stress, Detox (Topical + Internal)
- Powerful search and filters
- Modular data packs (easy to expand)

## Project Structure

```
kitchen-book/
├── index.html          # Main app
├── css/
│   └── styles.css
├── js/
│   └── app.js
├── data/
│   ├── manifest.json
│   ├── italian.json
│   ├── french.json
│   ├── chinese.json
│   ├── japanese.json
│   ├── thai.json
│   ├── korean.json
│   ├── indian.json
│   ├── mexican.json
│   ├── mediterranean.json
│   ├── american.json
│   ├── world.json
│   └── holistic.json
└── README.md
```

## How to Run

### Option 1 — Local server (recommended)
```bash
cd kitchen-book
python3 -m http.server 8000
```
Then open: http://localhost:8000

### Option 2 — GitHub Pages
1. Push this repo to GitHub
2. Settings → Pages → Deploy from main branch
3. Your app will be live at `https://<user>.github.io/<repo>/`

### Option 3 — Double-click (limited)
Opening `index.html` directly may block `fetch` due to browser CORS. Use a local server for full functionality.

## Expanding the Library

1. Add new recipes to the appropriate `data/*.json` file
2. Update the `count` in `data/manifest.json`
3. The app will automatically pick them up

Each recipe object looks like:
```json
{
  "id": "it21",
  "name": "Recipe Name",
  "style": "Home",
  "meal": "Dinner",
  "diet": ["Vegetarian"],
  "time": "30 min",
  "diff": "Easy",
  "tags": ["pasta"],
  "ingredients": ["Pasta", "Garlic"],
  "steps": ["Step 1", "Step 2"]
}
```

## License

Educational use. Recipes and remedies are for informational purposes. Always patch-test and consult professionals for health matters.

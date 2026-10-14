# Ninaivugal — responsive web companion

A polished, responsive browser version inspired by the user's Python/Kivy Ninaivugal app. This is a separate web implementation; it does not convert or replace the Android application.

## Run locally

Open `index.html` in a browser. For best testing, run a local static server from this folder:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Deploy free on Vercel

1. Create a GitHub repository and upload the **contents** of this folder (`index.html`, `style.css`, `script.js`, `assets/`, `README.md`).
2. Sign in to Vercel and import that repository.
3. Select **Other** as the framework preset. No build command is needed for this static website.
4. Deploy. Vercel provides a public HTTPS URL.

Alternative: GitHub Pages can host the static site from a repository's Pages settings.

## Included

- Responsive overview dashboard and custom illustrated hero
- Add/delete special days, recurring date countdowns, search and filters
- Memory journal linked to saved dates
- English/Tamil/Tanglish wish templates, tone choices, shuffle and copy
- JSON export/import backup and local-data clearing
- Mobile navigation and responsive layouts

## Important limitations

- This web companion saves data in this browser's `localStorage`. It does not sync with the Kivy Android app or other devices.
- Browser data may be cleared by the user/browser; export backups periodically.
- Wish generation uses built-in templates. It does not call Gemini or any AI service.
- The web version does not reproduce Android push notifications, PIN locking, or WhatsApp actions from the original app.
- Do not use a client-side API key in a public website. To add AI, create a server-side API proxy that protects the key.

# fuzzyqbit.github.io

Personal landing page listing my published GitHub projects.

## Deploy

1. Create a public repo on GitHub named **`fuzzyqbit.github.io`** (exact name — case matters for the URL).
2. Push these files:
   ```bash
   cd "/Users/rowan/Documents/fuzzyqbit.github.io"
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/fuzzyqbit/fuzzyqbit.github.io.git
   git push -u origin main
   ```
3. In the repo's **Settings → Pages**, set Source = `Deploy from a branch`, Branch = `main` / `root`. Save.
4. Wait ~1 minute. Site live at: **https://fuzzyqbit.github.io**

## Edit project descriptions

Open `index.html`, find each `<a class="card" ...>` block. Each card has:

- `<h2 class="card-title">` — project name
- `<p class="card-desc">` — short description
- `<span class="lang" data-lang="...">` — language label (auto-colors dot)

Replace the placeholder descriptions with your own. Add more cards by copying any `<a class="card">…</a>` block and incrementing the `card-index` (e.g. `09 / 09`) and updating the `.value` count in the hero.

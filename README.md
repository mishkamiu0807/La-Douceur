# La Douceur
A frontend-only coffee recipe app: 15 recipes, search and filters, serving scaling, a flavour quiz, an ingredient finder, a journal, and three themes. No build step.

## Run locally
Open `index.html` in a browser. Everything works from a file, though Google Fonts need a connection (system fonts are used otherwise).

## Deploy on GitHub Pages
1. Create a repository and upload `index.html` and `README.md`.
2. Go to Settings > Pages, choose "Deploy from a branch", pick `main` and `/ (root)`, and save.
3. Visit `https://USERNAME.github.io/REPO-NAME/` after a minute or two.

## Data
All data (favourites, tried recipes, journal, pantry, theme) is in your browser's localStorage under `amora.v1`. Use My Café > Export JSON for backups. Nothing syncs between devices.

## Customise
- Brand: edit `BRAND` at the top of the script.
- Colours: edit the CSS variables in `:root` and the `[data-theme]` blocks.
- Recipes: edit the `R` array. Each line is one recipe.
- Images: recipes use coloured tiles, so there are no external image dependencies.

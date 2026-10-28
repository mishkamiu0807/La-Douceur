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
- Images: see "Adding photos" below. Without photos the app shows coloured tiles.

## Adding photos
Create an `assets/` folder next to `index.html` and add JPGs with these exact names. Any missing file simply falls back to a coloured tile.

- `assets/hero-iced-latte.jpg` (about 1200x1200) and `assets/coffee-of-the-day.jpg` (about 800x600)
- `assets/recipes/` (about 800x600, under 150 KB each): `spanish-latte.jpg`, `strawberry-latte.jpg`, `lavender-honey-latte.jpg`, `caramel-macchiato.jpg`, `dirty-matcha.jpg`, `chocolate-mocha.jpg`, `orange-espresso-tonic.jpg`, `pistachio-cream-latte.jpg`, `vanilla-sweet-cream-cold-brew.jpg`, `coconut-cloud-coffee.jpg`, `brown-sugar-shaken-espresso.jpg`, `ube-latte.jpg`, `rose-latte.jpg`, `classic-affogato.jpg`, `dalgona-coffee.jpg`
- `assets/moods/` (about 600x800): `soft-girl-morning.jpg`, `study-fuel.jpg`, `rainy-day-reading.jpg`, `dessert-in-a-cup.jpg`, `summer-refresher.jpg`, `main-character-energy.jpg`, `slow-sunday.jpg`, `fancy-cafe-at-home.jpg`
- `assets/lifestyle/` (about 1200x400, banners): `paris-sunset-coffee.jpg` (quiz), `coffee-beans-bowl.jpg` (kitchen), `cozy-reading-bed.jpg` (journal), `cafe-interior-desk.jpg` (My Café), `journal-flatlay.jpg` (empty journal)

File names are case-sensitive on GitHub Pages. Upload the whole `assets` folder with the repository.


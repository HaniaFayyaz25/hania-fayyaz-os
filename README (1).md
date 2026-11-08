# Hania OS — haniafayyaz portfolio

My personal corner of the internet. A portfolio disguised as a warm little operating system: windows, a menu bar, a terminal, sticky notes on the fridge.

Live: https://hania-fayyaz-os.vercel.app (update this if your URL differs)

## What is inside
- **Desktop OS concept** — boot screen, live Lahore clock, scroll-spy menu bar, dock nav.
- **Work finder** — live client projects with filters, screenshots, and quick-view popups.
- **Journal** — real essays with strong opinions, readable in clean popups.
- **Hidden admin panel** — open `yoursite/#admin`, set a passphrase, add and edit projects and essays visually. Saves in the browser; export the backup to publish.
- **Playable terminal** — type under the prompt. `help` lists commands. `chai` three times for wisdom.
- **Project receipts + essay quote cards** — every project can print a shareable receipt PNG, every essay can become a square quote card, generated in the browser.
- **Guestbook fridge** — visitors stick notes on the fridge door.
- **Late-night mode** — visit between 11pm and 5am. The site gets warmer. Chai is on.

## Tech
Plain HTML, CSS, and JavaScript. No framework, no build step, no dependencies. Fonts load from Google Fonts. Fast on 3G by design.

## Run it locally
Open `index.html` in a browser. That is the whole setup.

## Update content
1. Open `yoursite/#admin` and edit work + journal visually.
2. Hit Email backup in the Backup tab.
3. Bake the JSON into `index.html` (`PROJECTS` and `POSTS` near the bottom) and push. Vercel redeploys on its own.

## Structure
- `index.html` — the entire site and app logic.
- `src/` — portrait, project screenshots, banners.

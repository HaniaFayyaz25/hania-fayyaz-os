# Hania Fayyaz Studio — Perchance Portfolio (Hania OS v2.0)

Warm OS concept: the whole site is a little operating system. Menu bar with live Lahore clock + scroll-spy app names, boot loader, window chrome (hello.txt, hello/, work/, about.png, Terminal, journal/, fridge/, now.txt, say-salam.mail), bottom dock nav, phone-notification stack.

## Files
- `main.pjs` — $meta + editable content lists (heroWord, quickNote, project1-6, studioWay, exploring). Edit text here.
- `index.html` — full OS: boot, menubar, windows, dock, filters by status (All/Live/Building), work quick-view modal, journal file rows + modal, copy email/WhatsApp, scroll spy.
- Hero word + quick note rotate with plain JS (same lists as main.pjs), so the page also works on Vercel where perchance `[list]` syntax does not evaluate. No other perchance syntax is used in index.html.
- `src/portrait-hania.jpg` — About portrait (Hania's niqabi photo).
- `src/work-*.jpg` — homepage screenshots for the 6 work cards (captured from the live sites).

## Contact links
- Email: haniafayyaz25@gmail.com
- WhatsApp: https://wa.me/923264566466
- LinkedIn: https://www.linkedin.com/in/hania-fayyaz-dev/

## Hidden admin panel
- Open `.../#admin` (or `.../#/admin`). First run sets a passphrase stored only in that browser.
- Tabs: Work (add/edit/delete projects), Journal (add/edit/delete writings, blank line = new paragraph), Backup (copy/download/email JSON to haniafayyaz25@gmail.com, import, reset to defaults, change passphrase, lock).
- Edits save to this browser instantly and survive reloads; counts and filters update automatically. To publish for everyone, send the Backup JSON to your developer. No link to the panel exists anywhere on the site.

## Invisible layer (homepage untouched, everything one click deep)
- Boot line: once a day, first load types "routing you in from {city} · {time}" from visitor timezone (no network). Stored day in localStorage.
- Late mode: 11pm to 5am visitor time adds body.late (warmer palette), swaps hello-note to "up late? chai is on.", shows mood dot in menubar.
- Presence: menubar "you are here" (desktop only); setPresence() hook + guarded createServerSocket check ready for live count after save + server script.
- Playable terminal: type under the prompt. Commands: help, whoami, work, journal, hire, rates, chai (rotates), salam/hello, sudo (joke), clear. Echo escaped, output capped at 40 lines, links clickable, 16px input to avoid iOS zoom.

## Click-deep layer (homepage untouched, everything inside existing popups + one fridge window)
- Receipts: work quick-view modal gets Visit/View-case/Receipt buttons; receipt view downloads a 480x640 PNG (order no, item, kind, status, wrapped stack, "paid in chai").
- Quote cards: journal modal gets "Make it a card"; uses highlighted text if selected, else longest strong sentence; downloads 1080x1080 PNG with Fraunces italic, date/tag, signature.
- Fridge: #fridge section (footer link + scroll spy), seeded notes + localStorage (cap 30), names/notes escaped, title counts notes, honest microcopy that shared fridge arrives with the saved version.
- Button contrast guard: .btn.btn-solid beige, .btn.btn-line terracotta (engine button rules were winning on some buttons).

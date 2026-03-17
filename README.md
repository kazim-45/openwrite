# FADE IN

**Professional screenwriting software. Free. Open source. Runs in your browser.**

[![Live Demo](https://img.shields.io/badge/live%20demo-fade--in--script--writer.vercel.app-c9a84c?style=flat-square)](https://fade-in-script-writer.vercel.app)
[![License](https://img.shields.io/badge/license-MIT-c9a84c?style=flat-square)](LICENSE)
[![Built With](https://img.shields.io/badge/built%20with-HTML%20%2F%20CSS%20%2F%20JS-c9a84c?style=flat-square)]()
[![Zero Dependencies](https://img.shields.io/badge/dependencies-zero-c9a84c?style=flat-square)]()
[![Deployed on Vercel](https://img.shields.io/badge/deployed%20on-Vercel-c9a84c?style=flat-square)](https://vercel.com)

---

FADE IN is a fully-featured, industry-standard screenwriting tool that runs as a single HTML file with zero dependencies, zero installation, and zero cost. Open it in a browser and start writing. It works on desktop, tablet, and mobile.

Built as a real alternative to WriterDuet and Celtx — without the paywall.

**[→ Open the app](https://fade-in-script-writer.vercel.app)**

---

## Features

### Screenplay Formatting Engine

Every element matches WGA industry-standard format precisely — margins, capitalization, spacing, and indentation are all correct out of the box.

| Element | Behavior |
|---|---|
| **Scene Heading** | All-caps, bold. Auto-detected when typing `INT.` or `EXT.` |
| **Action** | Full width, mixed case. Default element |
| **Character** | All-caps, centered. Auto-suggested from script history |
| **Parenthetical** | Italicized, auto-wrapped in parentheses |
| **Dialogue** | Narrower margins, standard screenplay column |
| **Transition** | All-caps, right-aligned. Auto-detected (`CUT TO:`, etc.) |

The `Enter` key is context-aware: Character → Dialogue, Scene Heading → Action, Transition → Scene Heading, and so on. `Tab` cycles through element types instantly.

---

### Smart Autocomplete

Suggestions appear as you type — no manual trigger required.

- Type `I` in a scene heading → suggests `INT.`, `INT./EXT.`, `I/E`
- Type `E` → suggests `EXT.`
- After `INT. LOCATION` + ` - ` → suggests `DAY`, `NIGHT`, `CONTINUOUS`, `LATER`, and more
- In a Character element → suggests every name already used in the script
- In a Transition element → suggests the full standard list (`CUT TO:`, `FADE OUT.`, `SMASH CUT TO:`, etc.)

Navigate with arrow keys. Confirm with `Tab`, `Enter`, or click.

---

### Script Doctor

A real-time analysis panel that monitors your script as you write and flags professional issues without interrupting your flow. Click any issue to jump the cursor directly to the offending line.

| Issue | What it checks |
|---|---|
| Missing `FADE IN:` | Scripts open with `FADE IN:` |
| Missing `FADE OUT.` | Scripts close with `FADE OUT.` or `THE END` |
| Long action block | Action over 4 lines slows pacing |
| Long monologue | Dialogue over 8 lines loses readers |
| `"We see"` / `"We hear"` | Describe directly — never address the reader |
| Scene missing time of day | Every heading needs `DAY`, `NIGHT`, `CONTINUOUS`, etc. |
| Passive voice | Action lines should use active, vivid verbs |
| No scene heading on page 1 | Every location needs a scene heading |

---

### Formatting Toolbar

Select any text and a floating toolbar appears above the selection — **Bold**, *Italic*, Underline, Strikethrough, and Clear formatting. Works on any element type. Fully supported on touch screens.

---

### Page System

- A4-proportioned page shell so the page always looks like a real sheet of paper
- Pages grow naturally as you write — no blank white space below your cursor
- Dashed page-break rulers with page numbers appear every 55 lines
- Live page count, word count, and scene count update in the navbar

---

### Sidebars

**Left — three tabs:**
- **Scenes** — live list of every scene heading; click any to jump directly to it
- **Characters** — auto-populated from every Character element in the script
- **Notes** — freeform scratchpad that saves alongside your script

**Right — Script Doctor** with clickable issue cards.

Both sidebars collapse on desktop. On mobile they become full-screen slide-over drawers.

---

### Export

**PDF** — `Ctrl+P` triggers a fully print-ready layout. All UI chrome is hidden. Browser headers and footers (URL, date, page number) are suppressed entirely via `@page { margin: 0 }`. The page shell provides proper screenplay margins. If a title page is configured, it prints as a separate first page.

**.txt / .fountain** — `Ctrl+S` downloads a plain-text file with proper screenplay indentation and spacing preserved.

---

### Title Page

Set via the **Title Pg** button — Title, Author, Based On, Draft, Date, Contact. The title page is stored separately and never shown in the editor. It appears automatically as the first page on every export.

---

### Persistence

- Autosaves to `localStorage` every 30 seconds
- On reload, detects a saved script and offers to restore it
- Live save status in the status bar

---

### Additional Features

| Feature | Detail |
|---|---|
| Dark / Light mode | `Ctrl+D` |
| Revision mode | Colors newly added lines in blue — industry standard |
| Focus mode | Hides all UI, leaves only the page |
| Find & Replace | Match count, next/previous navigation, replace one or all |
| Rotating placeholder | First-line placeholder cycles every 3 seconds when empty |

---

## Mobile

FADE IN is fully functional on phones and tablets. The layout adapts completely at ≤768px.

- **Navbar** — logo, title, and a hamburger `☰` button only
- **Bottom element bar** — all six element types as a sticky bar at thumb level
- **Drawer sidebars** — slide in from screen edges; swipe to dismiss
- **Hamburger menu** — bottom sheet with every feature: save, PDF, find, title page, revision mode, focus mode, theme, guide
- **Virtual keyboard handling** — bottom bar stays visible above the keyboard on iOS and Android
- **Swipe gestures** — swipe in from the left edge for scene navigator; right edge for Script Doctor
- **Touch formatting toolbar** — appears above text selections on touch screens

---

## Keyboard Shortcuts

| Action | Shortcut |
|---|---|
| Cycle element type | `Tab` |
| Smart new line | `Enter` |
| Confirm autocomplete | `Tab` / `Enter` |
| Navigate autocomplete | `↑` `↓` |
| Scene Heading | `Ctrl+1` |
| Action | `Ctrl+2` |
| Character | `Ctrl+3` |
| Parenthetical | `Ctrl+4` |
| Dialogue | `Ctrl+5` |
| Transition | `Ctrl+6` |
| Bold / Italic / Underline | `Ctrl+B` / `Ctrl+I` / `Ctrl+U` |
| Save as .txt | `Ctrl+S` |
| Export PDF | `Ctrl+P` |
| Find & Replace | `Ctrl+F` |
| Dark / Light mode | `Ctrl+D` |
| New scene heading | `Ctrl+Shift+N` |
| Focus mode | `Ctrl+Shift+F` |

---

## Format Reference

```
FADE IN:

INT. POLICE STATION - INTERROGATION ROOM - NIGHT

    A single bulb swings above a metal table. KHALID (30s,
    sharp eyes, exhausted) sits with his hands flat on
    the surface.

                        DETECTIVE RAZA
                  We found the car.

                        KHALID
                        (not looking up)
                  Then you already know everything.

                                            CUT TO:
```

---

## Tech Stack

| Layer | Choice |
|---|---|
| Language | Vanilla HTML / CSS / JS — zero build step |
| Font | Courier Prime via Google Fonts |
| Storage | `localStorage` |
| Hosting | Vercel |
| CI/CD | Push to `main` → live in ~20 seconds |

---

## Getting Started

**Use it instantly:**
```
https://fade-in-script-writer.vercel.app
```

**Run locally:**
```bash
git clone https://github.com/kazim-45/Fade-in-script-writer.git
cd Fade-in-script-writer
# Open index.html in any browser — no server needed
```

**Deploy your own:**
```
Fork this repo → connect to Vercel → done.
Vercel detects index.html automatically. No configuration required.
```

---

## Roadmap

- [ ] Next.js migration — component architecture
- [ ] Google authentication via NextAuth.js
- [ ] Cloud saves — Supabase (PostgreSQL) per-user script storage
- [ ] Script dashboard — list, rename, duplicate, delete
- [ ] Custom domain — `fadein.app`
- [ ] Real-time collaboration — Yjs / WebSockets
- [ ] Version history — named drafts, diff view
- [ ] React Native mobile app

---

## Contributing

Pull requests are open. If you find a formatting bug — wrong margins, wrong capitalization behavior, incorrect Tab/Enter flow — open an issue with the specific element type and the expected vs. actual behavior. For feature requests, check the roadmap first.

---

## License

MIT — use it, fork it, ship it. Credit appreciated, not required.

---

## Author

Built by **Kazim** — 17-year-old developer from Lahore, Pakistan.

[GitHub](https://github.com/kazim-45) · [Live App](https://fade-in-script-writer.vercel.app)

---

*FADE IN. Write something real.*

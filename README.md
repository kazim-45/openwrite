# OpenWrite

**Professional screenwriting software. Free. Open source. Runs in your browser.**

[![Live Demo](https://img.shields.io/badge/live%20demo-openwrite.vercel.app-c9a84c?style=flat-square)](https://openwrite.vercel.app)
[![License](https://img.shields.io/badge/license-MIT-c9a84c?style=flat-square)](LICENSE)
[![Built With](https://img.shields.io/badge/built%20with-HTML%20%2F%20CSS%20%2F%20JS-c9a84c?style=flat-square)]()
[![Zero Dependencies](https://img.shields.io/badge/dependencies-zero-c9a84c?style=flat-square)]()
[![Part of OpenSlate](https://img.shields.io/badge/part%20of-OpenSlate-c9a84c?style=flat-square)]()

---

OpenWrite is a fully-featured, industry-standard screenwriting tool that runs as a single HTML file. Zero dependencies. Zero installation. Zero cost. Open it in a browser and start writing.

Part of the **[OpenSlate](https://github.com/kazim-45)** suite — a free, open-source filmmaking toolkit.

**[→ Open the app](https://openwrite.vercel.app)**

---

## Features

### Screenplay Formatting Engine

Every element matches WGA industry-standard format — margins, capitalization, spacing, and indentation are all correct out of the box. The `Enter` key is context-aware throughout. `Tab` cycles element types instantly.

| Element | Format |
|---|---|
| **Scene Heading** | ALL-CAPS, bold. Auto-detected on `INT.` / `EXT.` |
| **Action** | Full width, mixed case |
| **Character** | ALL-CAPS, centered column |
| **Parenthetical** | Italic, auto-wrapped in parentheses |
| **Dialogue** | Standard screenplay column margins |
| **Transition** | ALL-CAPS, right-aligned. Auto-detected |

---

### Smart Autocomplete

Suggestions appear as you type — no trigger required.

- Type `I` in a scene heading → `INT.`, `INT./EXT.`, `I/E`
- Type `E` → `EXT.`
- After `INT. LOCATION -` → `DAY`, `NIGHT`, `CONTINUOUS`, `LATER`, and more
- In a Character element → every name used in the script so far
- In a Transition element → `CUT TO:`, `FADE OUT.`, `SMASH CUT TO:`, full standard list

Navigate with arrow keys. Confirm with `Tab`, `Enter`, or click.

---

### Script Doctor

Real-time analysis panel. Flags professional issues as you write without interrupting your flow. Click any issue to jump directly to the line.

| Flag | Rule |
|---|---|
| Missing `FADE IN:` | Scripts open with `FADE IN:` |
| Missing `FADE OUT.` | Scripts close with `FADE OUT.` or `THE END` |
| Long action block | Over 4 lines slows pacing |
| Long monologue | Over 8 lines loses readers |
| `"We see"` / `"We hear"` | Describe directly |
| Scene missing time of day | Every heading needs `DAY`, `NIGHT`, `CONTINUOUS`, etc. |
| Passive voice | Action lines need active verbs |
| No scene heading on page 1 | Every location needs a scene heading |

---

### Formatting Toolbar

Select any text and a floating toolbar appears — **Bold**, *Italic*, Underline, Strikethrough, Clear formatting. Works on every element type. Touch-screen supported.

---

### Page System

- A4-proportioned page shell — always looks like a real sheet of paper
- Pages grow naturally as you write
- Page-break rulers appear every 55 lines with page numbers
- Live page count, word count, and scene count in the navbar

---

### Sidebars

**Left sidebar:**
- **Scenes** — live list of every scene heading; click to jump
- **Characters** — auto-populated from every Character element
- **Notes** — freeform scratchpad, saves with the script

**Right sidebar — Script Doctor** with clickable issue cards.

Both collapse on desktop. On mobile they become full-screen slide-over drawers.

---

### Export

**PDF** — `Ctrl+P` opens a print-ready layout. All UI chrome hidden. Browser headers and footers suppressed via `@page { margin: 0 }`. If a title page is configured it prints as a separate first page with correct screenplay formatting.

**.txt / .fountain** — `Ctrl+S` downloads a plain-text file with proper screenplay indentation preserved.

---

### Title Page

Configured via the **Title Pg** button — Title, Author, Based On, Draft, Date, Contact. Stored separately from the editor. Never clutters your writing view. Prepended automatically on every export.

---

### Persistence

- Autosaves to `localStorage` every 30 seconds
- Detects and offers to restore a saved script on reload
- Live save status indicator

---

### Additional Features

| Feature | Shortcut |
|---|---|
| Dark / Light mode | `Ctrl+D` |
| Revision mode — new lines highlighted in blue | toolbar |
| Focus mode — hides all UI, just the page | `Ctrl+Shift+F` |
| Find & Replace with match count | `Ctrl+F` |

---

## Mobile

Fully functional on phones and tablets. The layout adapts completely at ≤768px:

- Navbar shows logo, title, and hamburger `☰` only
- Bottom element bar — all six element types at thumb level
- Sidebars become full-screen slide-over drawers; swipe to dismiss
- Hamburger menu — bottom sheet with every feature
- Virtual keyboard handling via `visualViewport` API
- Swipe in from screen edges to open sidebars
- Touch-aware formatting toolbar

---

## Keyboard Shortcuts

| Action | Shortcut |
|---|---|
| Cycle element type | `Tab` |
| Smart new line | `Enter` |
| Confirm autocomplete | `Tab` / `Enter` |
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
    the surface. DETECTIVE RAZA (40s) enters.

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
https://openwrite.vercel.app
```

**Run locally:**
```bash
git clone git@github.com:kazim-45/openwrite.git
cd openwrite
# Open index.html in any browser — no server needed
```

**Deploy your own:**
```
Fork this repo → connect to Vercel → done.
Vercel detects index.html automatically. No configuration required.
```

---

## OpenSlate Suite

OpenWrite is the first tool in the OpenSlate filmmaking suite.

| Tool | Description | Status |
|---|---|---|
| **OpenWrite** | Screenplay editor | ✅ Live |
| **OpenFrame** | Pre-production suite — storyboard, shot list, call sheet | ✅ Live |
| **OpenView** | Viewfinder and shot planning tool | 🔜 Coming |

The long-term vision: write your script in OpenWrite, plan your shoot in OpenFrame, frame your shots in OpenView — all connected, all free.

---

## Roadmap

- [ ] Import script into OpenFrame with one click
- [ ] Google authentication via NextAuth.js
- [ ] Cloud saves — Supabase per-user storage
- [ ] Script dashboard — list, rename, duplicate, version history
- [ ] Real-time collaboration
- [ ] Custom domain — `openwrite.app`

---

## Contributing

Pull requests are open. If you find a formatting bug — wrong margins, wrong capitalization behavior, incorrect Tab/Enter flow — open an issue with the specific element type and the expected vs. actual behavior.

---

## License

MIT — use it, fork it, ship it. Credit appreciated, not required.

---

## Author

Built by **Kazim** — 17-year-old developer and filmmaker from Lahore, Pakistan.

[GitHub](https://github.com/kazim-45) · [OpenWrite](https://openwrite.vercel.app) · [OpenFrame](https://openframe.vercel.app)

---

*FADE IN. Write something real.*

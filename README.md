# FADE IN
### Professional Screenwriting Software — Free, Open Source, Runs in Your Browser

![Version](https://img.shields.io/badge/version-1.0.0-c9a84c?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-c9a84c?style=flat-square)
![Built With](https://img.shields.io/badge/built%20with-vanilla%20HTML%2FCS%2FJS-c9a84c?style=flat-square)
![No Dependencies](https://img.shields.io/badge/dependencies-zero-c9a84c?style=flat-square)

---

**FADE IN** is a fully-featured, industry-standard screenwriting tool that runs entirely in a single HTML file. No installation. No subscription. No backend. Open the file — start writing.

Built as a real alternative to WriterDuet and Celtx for writers who want professional tools without the paywall.

---

## Demo

> Download `fade-in-web.html` → open in any browser → write your screenplay.

That's it.

---

## Features

### Core Writing Engine
- **All 6 screenplay elements** — Scene Heading, Action, Character, Parenthetical, Dialogue, Transition — each with pixel-perfect industry formatting
- **Smart `Enter` key** that knows context: Character → Dialogue, Scene Heading → Action, Transition → Scene Heading
- **Tab key** cycles through element types instantly
- **Line merging** on Backspace/Delete — behaves like a real word processor

### Smart Autocomplete
- Type `I` in a Scene Heading → dropdown offers `INT.`, `INT./EXT.`, `I/E`
- Type `E` → offers `EXT.`
- After `INT. LOCATION` + ` - ` → suggests `DAY`, `NIGHT`, `CONTINUOUS`, `LATER`, and more
- Character element → suggests every name already used in the script
- Transition element → suggests `CUT TO:`, `FADE OUT.`, `SMASH CUT TO:`, and the full standard list
- Navigate with arrow keys, confirm with Tab or Enter

### Formatting Toolbar
- Select any text → a floating toolbar appears with **Bold**, *Italic*, Underline, Strikethrough, and Clear formatting
- Works on any element type — character names, action lines, dialogue

### Script Doctor
A real-time analysis panel that flags professional issues as you write:
- Missing `FADE IN:` or `FADE OUT.`
- Action blocks over 4 lines
- Monologues over 8 lines
- `"We see"` / `"We hear"` in action lines
- Scene headings missing time of day
- Passive voice in action lines
- No scene heading on page one
- Click any issue to jump directly to the offending line

### Sidebars
- **Scene Navigator** — live list of every `INT./EXT.` heading; click to jump
- **Character List** — auto-populated from every CHARACTER element in the script
- **Notes Panel** — freeform scratchpad that saves with your script

### Page System
- Pages grow naturally as you write — no blank white space below your cursor
- Dashed page-break rulers appear at the correct intervals (every 55 lines)
- Page number displayed in the corner
- Page count, word count, and scene count updated live in the navbar

### Export
- **PDF** — `Ctrl+P` triggers a print-ready layout; all UI chrome hidden, screenplay page only
- **.txt / .fountain** — `Ctrl+S` downloads a properly spaced plain-text file with correct screenplay indentation

### Title Page
- Set via the **Title Pg** button — stores Title, Author, Based On, Draft, Date, Contact
- **Not inserted into your editor** — stays completely separate
- Prepended automatically on every export (PDF and .txt)

### Persistence
- **Auto-saves to localStorage** every 30 seconds
- On reload, detects a saved script and offers to restore it
- Save status shown live in the status bar

### Other
- **Dark / Light mode** — `Ctrl+D`
- **Revision Mode** — highlights newly added lines in blue (industry standard)
- **Focus Mode** — hides all UI, leaves only the page
- **Find & Replace** — with match count, next/previous navigation, replace one or all

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
| New Scene Heading | `Ctrl+Shift+N` |
| Focus mode | `Ctrl+Shift+F` |

---

## Screenplay Format Reference

```
INT. POLICE STATION - NIGHT

    Khalid sits alone at the interrogation table.
    A single light swings above him.

                        DETECTIVE RAZA
                  You were there. I know it.

                        KHALID
                        (quietly)
                  You don't know anything.

                                            CUT TO:
```

Every element — margins, capitalization, spacing — matches the WGA standard format used by working industry professionals.

---

## Tech Stack

| Layer | Technology |
|---|---|
| Language | Vanilla HTML, CSS, JavaScript |
| Font | Courier Prime (Google Fonts CDN) |
| Storage | localStorage |
| Dependencies | Zero |
| Build step | None |
| Bundle size | ~1 file |

This is intentionally zero-dependency. No React, no Node, no build pipeline. The entire application is one HTML file you can open offline, email to someone, or drop on any static host.

---

## Roadmap

The current version is a complete standalone tool. The next phase converts this into a full web application:

- [ ] **Next.js** — app framework, component architecture
- [ ] **Google Authentication** — via NextAuth.js, sign in with Google
- [ ] **Cloud saves** — Supabase (PostgreSQL) stores scripts per user, accessible from any device
- [ ] **Script dashboard** — list, rename, duplicate, delete scripts
- [ ] **Collaboration** — real-time co-writing (Yjs / WebSockets)
- [ ] **Custom domain** — `fadein.app`
- [ ] **Mobile app** — React Native port

---

## Getting Started

**Option 1 — Just use it:**
```
Download fade-in-web.html → Open in Chrome, Firefox, Safari, or Edge
```

**Option 2 — Clone and host:**
```bash
git clone https://github.com/YOUR_USERNAME/fade-in.git
cd fade-in
# Open FADE_IN.html in a browser — or drop it on any static host
```

**Option 3 — Deploy in 30 seconds:**

Drop `FADE_IN.html` into [Netlify Drop](https://app.netlify.com/drop) or any static hosting platform. Live instantly.

---

## Contributing

Pull requests are welcome. If you find a formatting bug — wrong margins, wrong capitalization logic, incorrect Tab/Enter behavior — open an issue with the specific screenplay element and expected behavior.

For feature requests: check the Roadmap above first. If your idea isn't there, open a discussion.

---

## License

MIT — use it, fork it, ship it. Credit appreciated, not required.

---

## Author

Built by **Kazim** — a 17-year-old builder from Lahore, Pakistan.

Filmmaker. Writer. Developer.

> *"The best screenwriting software is the one that gets out of your way."*

---

*FADE IN. Write something real.*

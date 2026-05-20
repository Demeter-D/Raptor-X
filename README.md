# Raptor X 30T — Operator Safety Briefing & Instruction Manual

A self-contained, single-file HTML manual for the **Raptor X 30-tonne PTO-driven
vertical log splitter**. Opens in any modern browser, online or offline. Works
on desktop and mobile (responsive layout for iPhone / Android).

---

## What's in this folder

| File          | Purpose                                                                                     |
|---------------|---------------------------------------------------------------------------------------------|
| `index.html`  | The full manual — 22 pages, all assets (machine photo, fonts, scripts) inlined. ~3–4 MB.    |
| `README.md`   | This file.                                                                                  |

That's it. No build step, no dependencies, no folders to keep in sync.

---

## How to open it

### On a computer
Double-click `index.html` and it opens in your default browser.

### On an iPhone / iPad
1. Copy `index.html` to iCloud Drive (or AirDrop it, or open from email).
2. Tap it from the **Files** app — it opens in Safari.
3. For best experience, tap the **Share** button → **Add to Home Screen**. The
   manual then behaves like a native app with no browser chrome.

### On a website (GitHub Pages, etc.)
Just upload `index.html` to the repository's root or a `/docs` folder, enable
GitHub Pages on that branch, and visit the published URL. No further setup
required — everything the page needs is already inside that one file.

---

## Using the manual

- **Scroll** through the 22 sections from cover to tear-off quick-reference.
- **Print / Save as PDF** — bottom-left "⎙ Print / Save PDF" button, or
  Cmd/Ctrl + P. The page is laid out to A4 with proper page breaks.
- **Tweaks panel** (bottom-right) lets you:
  - Change the document accent colour
  - Switch between Regular and Compact density
  - Toggle a "DRAFT" watermark across every page (for review prints)

On mobile, the multi-column layouts stack vertically and the type rescales for
phone reading. The watermark and right-hand checklist columns are hidden on
small screens since they only matter on print.

---

## What's inside

```
01  Cover & document identity
02  Contents & ANSI signal-word conventions
03  Machine specification
04  Component identification (annotated photo)
05  Decals & hazard symbols
06  Personal protective equipment
07  General safety rules
08  PTO shaft & entanglement
09  Hydraulic safety & injection injury
10  Work area & operating zones
11  Pre-start inspection
12  Hitching & PTO connection
13  Operating procedure
14  Log lift arm & log handling
15  Shutdown & disconnection
16  Transport & movement
17  Maintenance schedule
18  Hydraulic system service
19  Troubleshooting
20  Daily pre-start checklist
21  Operator briefing & sign-off
22  Tear-off quick reference
```

---

## Caveats — read before issuing

- Specifications (cylinder bore, hose lengths, exact reservoir capacity,
  operating mass, overall footprint, noise figure) are **typical industry
  values** for a 30 t PTO vertical splitter. Replace with the manufacturer's
  actual figures from your data plate / supplier sheet before distribution.
- Document number, revision and date on the cover are placeholders.
- This is generic operator safety guidance synthesised from PTO and hydraulic
  splitter best practice; it is not a substitute for the OEM's certified manual
  or a site-specific risk assessment carried out by a competent person.

---

## Editing the manual

`index.html` is a single self-contained file. To update content, open it in any
text editor (VS Code, Sublime, Notepad++) and search for the section heading
you need. The structure is plain HTML inside numbered `<section class="page">`
blocks — one section per printed page.

If you'd rather work with the unbundled source (separate JSX, asset folder,
etc.), ask for the un-inlined project files.

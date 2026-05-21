# Raptor X 30T — Operator Manual (deploy package)

Standalone HTML manual with favicon, app icons, OG/Twitter share image,
and a PWA manifest so it installs to a phone home-screen.

## Files

| File | Purpose |
|---|---|
| `Raptor X 30T - Operator Manual.html` | The manual itself |
| `tweaks-panel.jsx` | Tweaks panel runtime |
| `manifest.manual.json` | PWA manifest (paper background, ink theme) |
| `assets/raptor-x-30t.png` | Hero photograph used on cover + components page |
| `manual-icons/favicon-16.png` | 16×16 favicon |
| `manual-icons/favicon-32.png` | 32×32 favicon |
| `manual-icons/icon-192.png` | Android home-screen icon |
| `manual-icons/icon-512.png` | Large home-screen / splash icon |
| `manual-icons/icon-maskable-512.png` | Android adaptive icon (safe-area aware) |
| `manual-icons/apple-touch-icon.png` | iOS home-screen icon (180×180) |
| `manual-icons/og-image.png` | 1200×630 social sharing image |

## Hosting on GitHub Pages

Drop these files alongside the existing video files. The manual references
its icons and the photo by relative paths, so deeper folder structures work
fine — but keep `manual-icons/` and `assets/` as subfolders.

If the manual sits in a subfolder (e.g. `/manual/`), update the absolute
URLs in the `og:image` and `twitter:image` meta tags to your full hosted
URL — social platforms (LinkedIn, Slack, WhatsApp) need absolute URLs.

Example, for a repo at `you.github.io/raptor-x/`:

```html
<meta property="og:image" content="https://you.github.io/raptor-x/manual-icons/og-image.png" />
<meta name="twitter:image" content="https://you.github.io/raptor-x/manual-icons/og-image.png" />
```

## Installing on a phone

1. Open the URL in Safari (iOS) or Chrome (Android).
2. Share → Add to Home Screen.
3. The icon shows the paper "RX MANUAL" mark — visually distinct from
   the safety-briefing video icon, so you can tell the two apart on
   the home screen at a glance.

## Sharing

When the URL is pasted into Slack, WhatsApp, LinkedIn, iMessage etc.
the platform will fetch the OG image (cover-style preview with the
hero photo, headline, spec stats, and danger strip) and unfurl it
as a rich link card.

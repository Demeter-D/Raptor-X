# Raptor X — Deploy Package (fresh icons + OG)

Upload **all of these files to the root** of your `Raptor-X` repo on GitHub
(replacing what's there). The structure should end up flat — no subfolders.

```
Raptor-X/
├── index.html
├── manifest.json
├── favicon.png
├── favicon-16.png
├── favicon-32.png
├── apple-touch-icon.png
├── icon-192.png
├── icon-512.png
├── icon-maskable-512.png
└── og-image.png
```

## What changed

The manual HTML's `<head>` now uses **absolute URLs** for every favicon, app
icon, manifest, and OG image — all pointing to
`https://demeter-d.github.io/Raptor-X/<filename>`. That's the only setup
that survives HTML bundling AND works for social-link crawlers.

## After uploading

- **Favicon** appears in the browser tab within a refresh (force-refresh with
  Cmd+Shift+R / Ctrl+Shift+R to bypass cache the first time).
- **OG card** — paste the URL into Slack / WhatsApp / iMessage and you'll see
  the hero image + headline preview. If a platform has cached the old empty
  preview, use a debugger to force re-fetch:
    - Facebook / WhatsApp / LinkedIn: <https://developers.facebook.com/tools/debug/>
    - Twitter / X: <https://cards-dev.twitter.com/validator>
    - All-in-one preview: <https://www.opengraph.xyz/>

## Why the previous build didn't work

The old `<head>` referenced icons as `manual-icons/favicon-32.png` —
relative paths under a subfolder. After bundling, those got inlined as
data-URLs in the HTML, but social crawlers and some browsers couldn't
fetch them as separate files. Absolute URLs + files-at-root fixes both.

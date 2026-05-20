# tinydot-studio.github.io

Static landing page for TinyDot — Hanoi-based indie puzzle studio.

Live at: https://tinydot-studio.github.io/

## Files

- `index.html` — landing page (hero, games, about, contact)
- `privacy.html` — privacy policy (required by Google Play + Admob)
- `styles.css` — single stylesheet, no build step
- `app-ads.txt` — IAB Tech Lab authorized seller declaration for Admob verification
- `hashi-icon.png` — Hashi Classic app icon (1024×1024)

## Local preview

```bash
cd tinydot-studio-website
python3 -m http.server 8000
# open http://localhost:8000
```

## Deployment

1. Create GitHub user account `tinydot-studio` (or use existing one)
2. Create public repo named exactly `tinydot-studio.github.io`
3. Upload all files in this directory to the repo root
4. Settings → Pages → Source: Deploy from a branch → `main` / `(root)` → Save
5. Wait 1–2 minutes for first build
6. Verify URL: https://tinydot-studio.github.io/app-ads.txt returns the record line

## Updating Play Console Website

After GitHub Pages is live:

- Play Console → Developer account → Account details → Contact details
- Field "Website" → paste `https://tinydot-studio.github.io`
- Save changes
- Wait up to 24h for Play Store public page to propagate
- Trigger Admob recrawl in Admob console → Verify app → "Check for updates"

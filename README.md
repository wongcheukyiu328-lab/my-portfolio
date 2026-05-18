# Rachel Wong — Portfolio

Personal portfolio site. Vanilla HTML, CSS and JS — no framework, no build step.

## Pages

| Page | Path |
| --- | --- |
| Home | `index.html` |
| Work index | `work.html` |
| AIR — case study | `projects/air.html` |
| AIR Kit — case study | `projects/air-kit.html` |
| crypto.com — case study | `projects/crypto-com.html` |
| Ant Bank — case study | `projects/ant-bank.html` |
| Paint (about) | `projects/paint.html` |

`resume.pdf` lives at the root and is downloaded by the Resume button across every page.

## Local preview

Open `index.html` directly in a browser, or serve the folder so relative paths and `download` attributes behave like production:

```bash
python3 -m http.server 8000
# → http://localhost:8000
```

## Deploy to Vercel

1. Push this folder to a GitHub repo.
2. Import the repo in Vercel — it auto-detects a static site, no build command needed.
3. Production branch builds on every push to `main`.

No environment variables, no framework presets. Vercel serves the files as-is.

## Notes

- Fonts load from Google Fonts and Fontshare (Geist, Inter, Stack Sans Headline, etc.) via `<link>` tags in each page's `<head>`.
- Images are PNG/JPG/SVG at the repo root and in `lego/`, `assets/`.
- The site uses cross-document view transitions where supported, falling back gracefully.

# Wafica Design — Coming soon

The public "coming soon" page for Wafica Design (event decoration).
Plain HTML + CSS, no JavaScript, no build. Hosted as static files on Netlify.

The back-office system lives in its own repo: `wafica-design-system`.

## Run locally

```
python3 -m http.server 8080
# open http://localhost:8080
```

## Before going live

Search `index.html`, `robots.txt` and `sitemap.xml` and replace:

| Placeholder | Change to |
|---|---|
| `https://waficadesign.com` | the real domain |
| `961XXXXXXXX` | the WhatsApp number (digits only, with country code) |
| `instagram.com/waficadesign` | the real Instagram handle |

## Deploy (Netlify)

1. New site from Git, pick this repo.
2. Leave build command empty, publish directory `.` (already set in `netlify.toml`).
3. Add the custom domain.

Security headers (CSP, HSTS, ...) and cache rules are in `netlify.toml`.

## Files

```
index.html        the page
styles.css        brand tokens, layout, animations
assets/fonts/     Cormorant Garamond + Inter (self-hosted, latin)
assets/brand/     WD monogram, wordmark, favicon, social preview image
```

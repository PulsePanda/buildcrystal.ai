# buildcrystal.ai — holding page

Static single-page placeholder for buildcrystal.ai. No build step, no framework.

## Files
- `index.html` — markup and copy
- `styles.css` — all styling

## Local preview
```bash
cd Projects/buildcrystal-site
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy
Drop the folder onto any static host:
- **Cloudflare Pages** — connect the directory, no build command, output = `/`
- **Vercel / Netlify** — same, framework preset "Other"
- **S3 / anything** — upload the two files

## Newsletter form
Wired to Austin's personal Substack (`austinvanalstyne.substack.com`) — one list covers Crystal + everything else Austin publishes. The form POSTs to `https://austinvanalstyne.substack.com/api/v1/free?nojs=true`; on submit, Substack redirects to its confirmation page. To switch pubs, replace the `<form action=...>` URL in `index.html`.

## Logo
Currently a unicode diamond (◆) as a placeholder for the wordmark. Swap for an SVG when the real mark exists.

## Copy source
Positioning reflects Crystal Agents (per `Crystal/Agents/STRATEGY.md` and `Crystal/CLAUDE.md`) — purpose-built AI agents deployed as virtual employees, not the deprecated personal-assistant framing.

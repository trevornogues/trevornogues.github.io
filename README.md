# trevornogues.github.io

User GitHub Pages site for <https://trevornogues.github.io>.

Static pages for trust/SEO crawlers (home, about, contact) plus Organization
JSON-LD. The interactive personal site is the Next.js app on Vercel
(<https://trevvnog.vercel.app>).

## SEO files

- `robots.txt` — allows crawlers and points at `sitemap.xml`
- `sitemap.xml` — list every public page; **update `lastmod` to the day you
  actually edit that page** (not the deploy day)
- `c405503cf41f635413203fcee78fb209.txt` — IndexNow key file
- `.github/workflows/indexnow.yml` — pings IndexNow after each push to `main`

## Security headers

GitHub Pages cannot set custom response headers from this repo. Real
`Content-Security-Policy`, `X-Frame-Options`, etc. need Cloudflare (or similar)
in front of `*.github.io`, or live on the Vercel app which already sends them.

Pages source: branch `main`, folder `/`.


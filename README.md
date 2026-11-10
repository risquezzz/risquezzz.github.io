# Portfolio — Cristóbal Rísquez

Static one-page portfolio for GitHub Pages. No build step, no dependencies, no trackers.

## Files

| File | Purpose |
|---|---|
| `index.html` | The page. Content, structure and structured data. |
| `styles.css` | All styling. |
| `robots.txt` | Allows crawlers, points to the sitemap. |
| `sitemap.xml` | Single URL sitemap. |

## Before publishing: replace these placeholders

Search for `YOUR` in `index.html`, `robots.txt` and `sitemap.xml`.

| Placeholder | Replace with |
|---|---|
| `YOURUSERNAME` | Your GitHub username (used in canonical, OG and JSON-LD URLs) |
| `YOURPROFILE` | Your LinkedIn slug, e.g. `cristobalrisquez` |
| `YOUR@EMAIL.COM` | Your email address |

Example: if your username is `crisrisquez`, every `https://YOURUSERNAME.github.io/`
becomes `https://crisrisquez.github.io/`.

## Option A — upload from the browser (no tools needed)

1. Create a repository at <https://github.com/new> named exactly `YOURUSERNAME.github.io`.
2. Set it to **Public**. Do not add a README (you will upload one).
3. In the empty repo, click **uploading an existing file**.
4. Drag the four files (`index.html`, `styles.css`, `robots.txt`, `sitemap.xml`).
5. Commit.
6. Go to **Settings → Pages**. Under *Build and deployment*, set Source = **Deploy from a branch**,
   Branch = **main**, folder = **/ (root)**. Save.
7. Wait 1–2 minutes. Your site is at `https://YOURUSERNAME.github.io/`.

## Option B — with Git installed

```bash
git init
git add .
git commit -m "Portfolio: SEO & GEO analyst"
git branch -M main
git remote add origin https://github.com/YOURUSERNAME/YOURUSERNAME.github.io.git
git push -u origin main
```

Then enable Pages in Settings → Pages as in step 6 above.

## After publishing

- [ ] Open the site and check the email and LinkedIn links work.
- [ ] Test on a phone (the layout collapses at 820px).
- [ ] Add the URL to your LinkedIn **Featured** section and to your headline.
- [ ] Submit `https://YOURUSERNAME.github.io/sitemap.xml` in Google Search Console.
- [ ] Check the page in <https://pagespeed.web.dev/> — it should score high; it is one HTML file and one CSS file.

## Editing content

Everything lives in `index.html`. The numbers in the case study come from
`IMETAL_GEO_Baseline_Ronda2.xlsx`:

- AI Visibility 40/90 = 44.4%
- Recommendation per mention 30/40 = 75.0%
- Citation Rate 22/90 = 24.4%
- By intent: 66.7 / 56.7 / 30.0 / 26.7

If the dataset changes, update those four blocks and the table.

## Notes

- The `<script type="application/ld+json">` block declares you as a `Person` with
  `knowsAbout` and links the case study as an `Article`. Keep it: it is the part of
  the page that AI crawlers can parse as an entity.
- No JavaScript is used. Nothing to break, nothing to block.

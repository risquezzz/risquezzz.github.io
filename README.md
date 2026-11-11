# Cristóbal Rísquez — SEO & GEO Analyst

Personal portfolio and applied research on how brands appear in AI-generated answers.

**Live site:** https://risquezzz.github.io/

---

## What this repository contains

Three artefacts built from a single measurement project, plus the methodology behind them.

| Path | What it is |
|---|---|
| `index.html` | Portfolio landing page |
| `report/` | GEO visibility baseline for IMETAL, C.A. — 90 observations across ChatGPT, Gemini and Perplexity, in English and Spanish, as HTML and PDF |
| `audit/` | Technical SEO audit of the same site — structured data, performance, duplicate hosts, content architecture, in English and Spanish |
| `dashboard/` | Interactive view of the 90-observation dataset, plus `data.csv` with the raw table |
| `styles.css` | Styling for the landing page |
| `robots.txt`, `sitemap.xml` | Crawler directives and URL index |

## The project in one paragraph

IMETAL is an industrial pump and rotating-equipment repair company in El Tigre, Venezuela. I wrote 30 unbranded buyer prompts across four intents, ran each one in a fresh chat in three AI engines with memory disabled, and recorded 90 observations: full answer, mention, recommendation, cited URLs and competitors. Visibility came out at 44.4%, but the useful finding was the distribution — 66.7% on transactional prompts against 0 mentions across the six purely conceptual ones. The technical audit explains why: the site is a single page with a broken JSON-LD block, so there is nothing for an engine to retrieve or cite.

## Method, in short

1. Prompts written as real buying questions, with no brand name in any of them.
2. One fresh conversation per prompt, memory off, to keep observations independent.
3. Full answer captured per row, not a summary.
4. Three metrics kept separate: mention, recommendation, citation.
5. All 40 mentions reviewed by hand; an automatic rule over-counted by eight.
6. Limits stated before conclusions: single day, three of four surfaces, undisclosed model versions.

## Data

`dashboard/data.csv` is the fact table: 90 rows, one per prompt × engine, with binary flags for mention, recommendation and citation.

The consolidated workbook, the raw answers and the competitor inventory live outside this repository, in the project folder. The numbers published on the site all trace back to that workbook.

No client-confidential information is included. Everything published comes from public AI outputs and public web data.

## Technical notes

- Static HTML and CSS. No framework, no build step, no JavaScript on the landing page.
- JSON-LD on the landing page declares the author as a `Person` with `knowsAbout`, and the case study as an `Article`.
- Report and audit pages are generated from Markdown sources, then printed to PDF.
- Deployed with GitHub Pages from the `main` branch.

## Local preview

Clone the repository and open `index.html` in a browser. Relative links between sections work from disk; the PDFs open locally as well.

## Contact

- Email: cristobalrisquez.1@gmail.com
- LinkedIn: https://www.linkedin.com/in/crist%C3%B3bal-r%C3%ADsquez-a76523441/

# Orchid Internships

The program site, handbook, and operational artifacts for the Orchid Internship Program.

## What lives here

| Path | Purpose |
|---|---|
| `docs/` | Public website — served at our GitHub Pages URL |
| `.github/ISSUE_TEMPLATE/` | Host Problem Brief and Intern Profile forms (coming) |
| `handbook/` | CLAUDE.md template, pair-repo template, Problem Brief template (coming) |

## Local preview

```sh
cd docs
python3 -m http.server 4173
```

Then open http://localhost:4173/.

## Deploying

The site is plain HTML/CSS — no build step. GitHub Pages serves `docs/` on push to `main`.

To enable Pages the first time:

1. Go to **Settings → Pages**
2. Under **Build and deployment**, set **Source** to *Deploy from a branch*
3. Set **Branch** to `main` and **Folder** to `/docs`
4. Save

Once live, point a custom domain (e.g. `internships.orchid-initiative.com`) at it via the Pages settings and a DNS CNAME record.

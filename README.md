# Idira — Platform Notes

A static, 6-page reference site covering the Idira identity security platform:

1. `blueprint.html` — Idira Blueprint
2. `risk-management.html` — Idira Risk Management
3. `itdr.html` — Idira ITDR
4. `discovery-saas.html` — Discovery SaaS
5. `ispss-whats-new.html` — Idira ISPSS Platform: What's New
6. `cora-ai.html` — CORA AI

No build step, no dependencies beyond a Google Fonts CDN link in `assets/style.css`. Pure HTML/CSS/JS.

## Host it on GitHub Pages (free)

**1. Create a repo**
On GitHub, click **New repository**. Name it anything (e.g. `idira-notes`). Public repos get free Pages hosting; private repos need GitHub Pro/Team/Enterprise for Pages.

**2. Upload the files**
Easiest path if you don't use git day-to-day:
- Open your new repo → **Add file → Upload files**
- Drag in `index.html`, `blueprint.html`, `risk-management.html`, `itdr.html`, `discovery-saas.html`, `ispss-whats-new.html`, `cora-ai.html`, `README.md`, and the whole `assets/` folder (drag the folder itself, GitHub preserves the structure)
- Commit directly to `main`

Or via git from your terminal:
```bash
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo>.git
git push -u origin main
```

**3. Turn on Pages**
Repo → **Settings → Pages** → under "Build and deployment", set **Source** to **Deploy from a branch** → **Branch: main**, folder **/ (root)** → **Save**.

**4. Visit your site**
GitHub will show a URL like `https://<your-username>.github.io/<your-repo>/` — it usually goes live within a minute or two (sometimes up to ~10 minutes on the first deploy).

## Notes

- All content is paraphrased from public sources (Palo Alto Networks / CyberArk product pages and docs) as of August 2026 — verify anything time-sensitive (like the "What's New" page) against the official docs before relying on it.
- The footer disclaimer noting this is an independent, unofficial reference is intentional — keep it if you publish this publicly.
- To add a custom domain, see GitHub's docs on "Managing a custom domain for your GitHub Pages site."

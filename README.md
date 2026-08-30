# Nils Handler — Academic Website

Built with [Jekyll](https://jekyllrb.com/) and the [al-folio](https://github.com/alshedivat/al-folio) theme. Hosted on GitHub Pages.

## Quick Setup

### 1. Fork al-folio
Go to [github.com/alshedivat/al-folio](https://github.com/alshedivat/al-folio) and click **Fork**.  
Rename the repo to `<your-github-username>.github.io`.

### 2. Copy these files into your fork
Replace/add the following from this folder:
- `_config.yml` — update `url`, `github_username`, `orcid_id` once you have them
- `_pages/about.md` — your main landing page
- `_pages/publications.md`
- `_pages/talks.md`
- `_pages/cv.md`
- `_pages/teaching.md`
- `_bibliography/papers.bib` — your publications
- `_news/announcements.yml` — news items
- `assets/css/custom.scss` — video embed styles

### 3. Add your photo
Upload `assets/img/prof_pic.jpg` — this is your profile photo (already named correctly for al-folio).

### 4. Add your CV PDF
Upload `assets/pdf/Nils_Handler_CV.pdf`.

### 5. Update _config.yml
Edit these fields:
```yaml
url: https://<your-github-username>.github.io
github_username: <your-github-username>
orcid_id: <your-orcid-id>          # after registering at orcid.org
scholar_userid: <google-scholar-id> # optional
```

### 6. Enable GitHub Pages
In your repo → Settings → Pages → Source: **GitHub Actions**.  
Al-folio includes a `.github/workflows/deploy.yml` that handles the build automatically.

### 7. Local preview (optional)
```bash
bundle install
bundle exec jekyll serve
# open http://localhost:4000
```

## File Structure
```
_bibliography/papers.bib     ← Add publications here (BibTeX)
_data/socials.yml            ← Social/contact links
_news/announcements.yml      ← News items (shown on homepage)
_pages/about.md              ← Homepage
_pages/publications.md       ← Publications page
_pages/talks.md              ← Talks & videos
_pages/cv.md                 ← CV page
_pages/teaching.md           ← Teaching page
assets/css/custom.scss       ← Custom styles (video embeds etc.)
assets/img/prof_pic.jpg      ← Profile photo ← ADD THIS
assets/pdf/Nils_Handler_CV.pdf ← CV PDF ← ADD THIS
```

## Adding a new publication
Edit `_bibliography/papers.bib` and add a BibTeX entry. Set `selected = {true}` to show it on the homepage.

## Adding news
Edit `_news/announcements.yml` and add a new entry at the top:
```yaml
- date: 2026-06-01
  inline: Your news item here.
```

# Minwoo James Kim

Personal academic website, built with Jekyll and published to GitHub Pages.

## Content

- `_data/cv.json`: shared research, publications, talks, software, education, honors, and leadership records.
- `assets/pdf/cv_mjkim.pdf`: current downloadable CV.
- `index.md`: short home-page introduction.
- `_pages/`: Research, Publications & Talks, Selected Software, Background, and legacy URLs.
- `_includes/`: content sections shared by the dedicated pages and the full `/cv/` view.
- `_layouts/default.html` and `assets/css/site.css`: shared navigation, layout, and responsive styles.

Update shared records in `_data/cv.json` when updating the CV. The home-page publication announcement is edited separately in `index.md`.

## Local development

Use Ruby 3.3, then run:

```sh
bundle install
bundle exec jekyll serve
```

To verify the production build:

```sh
JEKYLL_ENV=production bundle exec jekyll build
```

Pushing to `main` runs `.github/workflows/pages.yml` and deploys the generated `_site` directory. Older `/talks/`, `/projects/`, `/cv/`, and `/projects/vqnhe/` URLs remain available.

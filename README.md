# mmugilan.github.io

Source for my personal website, [mmugilan.github.io](https://mmugilan.github.io), built with Jekyll and hosted on GitHub Pages.

## Editing content

Most content lives in YAML files under `_data/`:

- `publications.yml`: papers and their links
- `talks.yml`: talks
- `experience.yml`: roles
- `profile.yml`: education, awards, and service

The pages are `index.html`, `publications.html`, `experience.html`, and `404.html`. The shared frame is `_layouts/default.html`, and all styles are in `assets/css/site.css`. PDFs (CV, papers, slides) and images go in `static/`. `_archive/` holds old photos and is not published.

## Running locally

Needs Ruby 3.3.6 (see `.ruby-version`). Gems install into `vendor/bundle` inside the repo, not globally.

```bash
bundle config set --local path vendor/bundle
bundle install
bundle exec jekyll serve
```

Then open http://127.0.0.1:4000. Pushing to `main` publishes the site.

## License

Site text: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Papers and slides: their publishers' terms. Code: MIT, see [LICENSE.md](LICENSE.md).
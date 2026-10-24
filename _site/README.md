# Kaffeinated Kodemonkey

The source repository for [kaffeinatedkodemonkey.com](https://www.kaffeinatedkodemonkey.com), a Jekyll site about digital accessibility services, WCAG, testing, and compliance.

## Technology

- Jekyll 4.3, Ruby 3.3.4, and Liquid templates
- Minima as the base theme, with custom layouts, includes, CSS, and JavaScript
- `jekyll-feed`, `jekyll-seo-tag`, and `jekyll-admin` plugins
- Bootstrap and other front-end libraries vendored under `assets/vendor/`

## Run locally

Install the Ruby version listed in `Gemfile`, then install the project gems and start Jekyll:

```sh
bundle install
bundle exec jekyll serve
```

Open the local URL printed by Jekyll (usually `http://127.0.0.1:4000`). To build the static site without serving it:

```sh
bundle exec jekyll build
```

The generated site is written to `_site/`. Jekyll serves changes to most content and template files automatically. Restart the server after changing `_config.yml`.

## Site structure

- `index.markdown` — homepage
- `about.html`, `services/`, and `a11y_policy/` — company, service, and policy pages
- `monkeyhub/` — Articles & News, Learning Center, resources, and support pages
- `topics/` — Learning Center topic landing pages
- `_posts/learning_center/` — accessibility guides
- `_posts/learning_center/wcag_series/` — the beginner WCAG series
- `_posts/articles/` — articles and industry updates
- `_layouts/` and `_includes/` — page layouts and reusable Liquid components
- `_data/` — structured site data, including sidebar links and SEO content planning
- `assets/` — stylesheets, scripts, images, documents, and vendored libraries
- `_templates/` — reference templates for drafting content

## Content conventions

Add published articles and guides to the appropriate `_posts/` subdirectory. Use a date-prefixed filename (`YYYY-MM-DD-title.md`) and valid YAML front matter. Post front matter should include `layout`, `title`, a concise `description` under 160 characters, and `tags`; follow the conventions in neighboring posts for categories and permalinks. Keep existing permalink patterns stable when editing published content.

Use descriptive alternative text for informative images. Use empty alt text (`alt=""`) for decorative images. When adding images in Markdown, include meaningful alt text in the image syntax.

## Configuration and SEO

Site-wide settings, canonical URL, permalink pattern, and plugins are in `_config.yml`. The site uses `jekyll-seo-tag` for metadata and `jekyll-feed` for its feed. Update shared sidebar links in `_data/sidebar.yml`.

## Deployment

Build the site with `bundle exec jekyll build` and deploy the generated `_site/` directory using the hosting workflow configured for the project. The repository does not currently document a specific CI deployment workflow.

# Yifan Zhang — Personal Website

Source for [1phan.com](https://1phan.com), built with Jekyll and the
[Academic Pages](https://github.com/academicpages/academicpages.github.io) theme.

## Site structure

| Page | Source | URL |
| --- | --- | --- |
| Homepage | `_pages/about.md` | `/` |
| Selected Publications | `_pages/publications.md` | `/publications/` |
| Blog | `_pages/blog.html` | `/blog/` |
| Not found | `_pages/404.md` | `/404.html` |

`about.md` is the homepage and contains the biography, research interests,
publications grouped by research domain, professional service, news, and selected awards.
The Selected Publications page lists full citations by year, PDF links, and
expandable research impact descriptions. The homepage links to this detailed page.
Professional service remains a section on the homepage.
`/about/`, `/about.html`, and `/services/` redirect to `/`.
The standalone teaching page has been removed.

The site title links back to the homepage; navigation links are maintained in
`_data/navigation.yml`.

Blog posts live in `_posts/`. PDFs are in `files/`, and the profile photo and
blog illustrations are in `images/`. Site-wide settings are in `_config.yml`.
The XML sitemap and RSS feed are generated automatically.

The template demo pages, placeholder collections, sample comments, and duplicate
archives have been removed. Blog is the single post archive; tag and category
archive links are disabled. Publication details are maintained in
`_pages/publications.md`; the brief research-domain overview and professional
service are maintained in `_pages/about.md`. The optional `markdown_generator/`
utilities are retained for reference and excluded from the published website.

## Local preview

With Ruby and Bundler installed:

```sh
bundle install
bundle exec jekyll serve
```

Open `http://localhost:4000`. To check a production build:

```sh
JEKYLL_ENV=production bundle exec jekyll build
```

Restart the preview server after changing `_config.yml`.

## Theme credit

Academic Pages is based on the Minimal Mistakes theme. See `LICENSE` for the
original MIT license.

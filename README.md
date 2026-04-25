# jaxsenrday academic site

This repository is set up as a lightweight GitHub Pages academic website for Jaxsen R. Day.

With the current repository name, the published site URL will be:

- `https://jaxsenday.github.io/jaxsenrday/`

## How it works

- The site is designed to publish directly from GitHub Pages with no local build step required.
- Most of the content lives in [`_data/site.yml`](/Users/jaxsen/Documents/GitHub/jaxsenrday/_data/site.yml).
- The page structure is kept simple so it is easy to update with Codex or by editing text files directly.

## Main files

- [`_data/site.yml`](/Users/jaxsen/Documents/GitHub/jaxsenrday/_data/site.yml): biography, links, papers, talks, activities, and contact info
- [`index.md`](/Users/jaxsen/Documents/GitHub/jaxsenrday/index.md): homepage
- [`papers.md`](/Users/jaxsen/Documents/GitHub/jaxsenrday/papers.md): papers page
- [`activities.md`](/Users/jaxsen/Documents/GitHub/jaxsenrday/activities.md): talks, service, teaching, and awards
- [`cv.md`](/Users/jaxsen/Documents/GitHub/jaxsenrday/cv.md): CV page
- [`contact.md`](/Users/jaxsen/Documents/GitHub/jaxsenrday/contact.md): contact page

## Typical updates

1. Edit `_data/site.yml`
2. Commit the changes
3. Push to GitHub
4. GitHub Pages republishes the site

## Local preview

This repo can be built locally with the GitHub Pages gem through Bundler. On this Mac, use Homebrew Ruby 3.3:

```bash
env BUNDLE_PATH=vendor/bundle /opt/homebrew/opt/ruby@3.3/bin/bundle install
env BUNDLE_PATH=vendor/bundle /opt/homebrew/opt/ruby@3.3/bin/bundle exec jekyll build
env BUNDLE_PATH=vendor/bundle /opt/homebrew/opt/ruby@3.3/bin/bundle exec jekyll serve
```

The generated `_site`, `.jekyll-cache`, and `vendor/bundle` folders are ignored by Git.

## Optional future cleanup

If you later rename the repository to `jaxsenday.github.io`, it can become your main user site at:

- `https://jaxsenday.github.io/`

## Next content to add

- Your LinkedIn profile URL
- Paper, presentation, or project links you want to make public
- A finalized public CV file when you are ready to publish one

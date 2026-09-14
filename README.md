# web

Hosting for simple static pages and things built with Claude (artifacts, one-off pages, small tools) &mdash; served free via GitHub Pages.

## Live site

Once Pages is enabled (see below), this repo is served at:

```
https://snottledev.github.io/web/
```

## Adding a new page

Give each page its own folder with an `index.html` inside, e.g.:

```
/my-project/index.html   ->  https://snottledev.github.io/web/my-project/
```

Then add a link to it from the root `index.html` so it's discoverable from the homepage.

For a single self-contained HTML file (no separate assets), it's fine to drop it directly in a folder as `index.html`; keep any CSS/JS/images inside that same folder if a page needs more than one file.

## One-time setup: enable Pages

GitHub Pages isn't on by default for a new repo &mdash; this has to be clicked once in the UI (no API for it via this setup):

1. Go to **[github.com/snottleDev/web/settings/pages](https://github.com/snottleDev/web/settings/pages)**
2. Under **Build and deployment > Source**, choose **Deploy from a branch**
3. Branch: **main**, folder: **/ (root)**
4. Save

It takes a minute or two to go live the first time; after that, every push to `main` updates the site automatically.

## Notes

- `.nojekyll` disables GitHub's default Jekyll processing, so folders/files starting with `_` (common in some build tools) aren't ignored.
- This repo is public, which is required for free GitHub Pages hosting on a personal account.

# mohammadsayyadi.com

Personal academic website. Static HTML/CSS, no build step or dependencies.

## Structure

```
index.html          Home / about
research.html        Dissertation and works in progress
publications.html    Book chapters and peer-reviewed articles
teaching.html         Teaching experience
contact.html          Email, Google Scholar, office address
images/                Headshot and personal photos (index.html only)
```

## Fonts

Loaded from Google Fonts via `<link>` in each page's `<head>`:
- **Fraunces** — display / headings
- **Source Serif 4** — body text
- **Inter** — navigation, labels, captions

## Deploying with GitHub Pages

1. Push this repo to GitHub.
2. In the repo settings, under **Pages**, set the source to the `main` branch, root folder.
3. The site will be live at `https://<username>.github.io/<repo-name>/`.

For a custom domain (e.g. `mohammadsayyadi.com`), add a `CNAME` file at the repo root containing the domain, and point your domain's DNS to GitHub Pages per [GitHub's custom domain docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).

## Editing

All five pages share the same design tokens (colors, fonts, spacing) defined inline in each page's `<style>` block. There's no shared stylesheet by design — each file is self-contained and can be opened directly in a browser without a server.

To update content, edit the HTML directly. Navigation links are relative (`research.html`, `contact.html`, etc.), so the site works whether it's served from a domain root or a GitHub Pages subpath.

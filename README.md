# Low Resource Computing — website

Hugo site for the [Low Resource Computing](https://lrc.cs.dartmouth.edu) workshop, deployed to GitHub Pages.

## Develop

```
hugo server -D
```

## Structure

- `content/` — page content (Markdown + front matter)
- `content/previous/2025/` — frozen archive of the 2025 site, rendered with its own standalone styling (`layouts/archive/`)
- `layouts/` — project-level templates (no external theme)
- `assets/css/main.css` — site stylesheet, processed via Hugo Pipes (minified + fingerprinted)
- `static/CNAME` — custom domain for GitHub Pages

## Deploy

Pushes to `main` build and deploy automatically via `.github/workflows/hugo.yml` to GitHub Pages. Repo Settings → Pages → Source must be set to "GitHub Actions".

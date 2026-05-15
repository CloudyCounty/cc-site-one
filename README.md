# Cloudy County Community Calls — Hugo Site

A Hugo site built on the [Stack theme](https://github.com/CaiJimmy/hugo-theme-stack) that publishes the 10 most recent recordings from the **Cloudy County Community Calls** YouTube playlist.

## What's in this folder

- `config/_default/` — Site configuration, customized for Cloudy County (title, sidebar, footer, social links).
- `content/_index.md` — Home page menu entry.
- `content/post/` — One folder per video. Each `index.md` embeds the YouTube video and includes a description, categories, and tags.
- `content/categories/` — Seven categories: Copilot, Teams, Forms & Lists, Outlook, Viva, SharePoint, and M365 Updates.
- `content/page/` — About, Archives, Links, and Search pages.
- `assets/`, `.github/workflows/`, `go.mod`, `go.sum` — Inherited from the starter, unchanged.
- `build_site.py` — The generator script used to produce the posts and categories. Safe to delete once you're happy with the content.

## Before you deploy

1. Confirm `baseurl` in `config/_default/config.toml` matches your GitHub Pages URL.
2. Replace `assets/img/avatar.png` and `assets/img/favicon.png` with your own Cloudy County branding.
3. (Optional) Drop a `cover.jpg` into each `content/post/<slug>/` folder — the theme will auto-detect it as the post cover image.
4. The July 2025 post (video ID `m8nd991XYrQ`) has only a partial description because the full YouTube text wasn't recoverable when this site was generated. Paste the full description into `content/post/2025-07-teams-meetings-updates/index.md` if you'd like.

## Local preview

```bash
hugo mod get -u
hugo server
```

The original Stack-theme starter README for the upstream template is preserved on the [hugo-theme-stack-starter repo](https://github.com/CaiJimmy/hugo-theme-stack-starter).

[![Gist](https://img.shields.io/badge/gist.github-version_of_this_repository-DCDCDC?style=for-the-badge&logo=github)](https://gist.github.com/OstinUA/7d82c337e3402ec9771d3ed23fab64cb)

[![Chrome Store](https://img.shields.io/badge/platform-Chrome_Extension-4285F4?style=for-the-badge&logo=google-chrome&logoColor=white)](https://chromewebstore.google.com/search/OstinUA)
[![Chrome Portfolio](https://img.shields.io/badge/Chrome_Web_Store-Portfolio-34A853?style=for-the-badge&logo=google-chrome&logoColor=white)](https://ostinua.github.io/Chrome-Web-Store_Developer-List/)

# My Chrome Extensions — GitHub Pages site

Jekyll-powered portfolio for Chrome extensions, deployed from the `/docs` folder.

## Structure

```
docs/
├── _config.yml              # Jekyll config + profile data
├── _data/
│   ├── extensions.yml       # Extension cards (add/edit here)
│   └── marquee.yml          # Scrolling strip items
├── _includes/
│   ├── header.html          # Sticky header + theme toggle + GitHub link
│   ├── profile.html         # Avatar + bio block
│   ├── marquee.html         # Auto-scrolling strip
│   └── extensions.html      # Grid of extension cards
├── _layouts/
│   └── default.html         # Base layout
├── assets/
│   ├── css/style.css
│   └── js/theme.js          # Theme toggle (with localStorage)
└── index.html               # Home page
```

## Deploy to GitHub Pages

1. Push this `docs/` folder to the repo.
2. Repo **Settings → Pages**.
3. **Source:** Deploy from a branch.
4. **Branch:** `main` (or `master`), **folder:** `/docs`.
5. Save. The site will be published at `https://<username>.github.io/<repo>/`.

If deploying to a user/org site (`<username>.github.io`), `baseurl` can stay empty.
If deploying to a project site, uncomment `baseurl` / `url` in `_config.yml` and set them accordingly.

## Editing content

- **Add an extension:** append a new entry to `_data/extensions.yml`.
- **Change profile text / avatar:** edit `profile:` section in `_config.yml`.
- **Change marquee items:** edit `_data/marquee.yml`.

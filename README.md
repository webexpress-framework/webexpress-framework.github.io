# WebExpress

`WebExpress` is a lightweight web server optimized for use in low-performance environments (e.g. Raspberry Pi). By providing a powerful plugin system and a comprehensive API, web applications can be easily and quickly integrated into a .NET language (e.g. C#). Some advantages of `WebExpress` are:

- It is easy to use.
- It offers a variety of features and tools that can help you build and manage your website.
- It is fast and efficient and can help you save time and money.
- It is flexible and can be customized to meet your specific requirements.

Landing page for the [WebExpress Framework](https://github.com/webexpress-framework/WebExpress), hosted on [GitHub Pages](https://webexpress-framework.github.io/webExpress-framework/).

The site introduces the framework's core concepts, documentation links, contribution guide and contact information. It is intentionally minimal — no external fonts, no analytics, no cookies, no CDN dependencies.

## Local preview

Open `site/index.html` directly in a browser, or serve the folder with any static file server:

```bash
python -m http.server --directory site 8080
```

Then open [http://localhost:8080](http://localhost:8080).

## Deployment

The site is deployed automatically via GitHub Actions whenever a change to `site/**` is pushed to `main`. The workflow:

1. Validates that no HTML file loads resources from external origins.
2. Uploads the `site/` folder as a GitHub Pages artifact.
3. Deploys it to GitHub Pages.

### Enable GitHub Pages (one-time setup)

Go to **Settings → Pages** in this repository and set the source to **GitHub Actions**. After the next push to `main` the site will be live at:

```
https://webexpress-framework.github.io/webExpress-framework/
```

## Design constraints

- No external resources — all fonts, images and scripts are served from the same origin.
- No cookies, no `localStorage`, no `sessionStorage`.
- System fonts only.
- Responsive, mobile-first, WCAG AA in mind.

## AI transparency notice

Parts of this software, its documentation, and its assets were created with the assistance of AI-based tools, including large language models. AI-assisted contributions are reviewed by the project maintainer before they are included.

## License

MIT — see [LICENSE](LICENSE).

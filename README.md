<p align="center">
  <img src="assets/logo.png" alt="My Morning News" width="420">
</p>

# mymorningnews.ai

Marketing website for [My Morning News](https://github.com/jchristn/MyMorningNews): sign up, tell us what you want to stay on top of, and let AI curate your regular news, as a podcast, an email, or in the app. Hosted on GitHub Pages at **[mymorningnews.ai](https://mymorningnews.ai)**.

## Development

Plain static site: no build step, framework, analytics, or third-party scripts. Serve the folder and open it:

```bash
python3 -m http.server 12192
```

Then browse to http://127.0.0.1:12192.

## Files

- `index.html`: the home page (hero, how it works, channels, features, pricing, self-hosting, FAQ).
- `privacy.html`, `terms.html`, `support.html`, `delete-account.html`: pages the app stores require (privacy, support, and account deletion URLs). The privacy policy and terms are alpha drafts for review.
- `404.html`: not-found page for GitHub Pages.
- `styles.css`: styling, with light and dark themes driven by CSS variables (dark follows the system, with a toggle).
- `script.js`: theme toggle and mobile menu.
- `assets/`: logo, glyph, favicons, and the Open Graph image, generated from the main repository's `assets/`.
- `CNAME`, `robots.txt`, `sitemap.xml`.

## Links into the app

Sign up and log in go to `https://app.mymorningnews.ai/signup` and `https://app.mymorningnews.ai/login`, the hosted service described in section 33 of the main repository's plan. App Store and Google Play badges are added when the mobile apps ship.

## Keeping it accurate

Product claims come from the main repository's README and `MY_MORNING_NEWS_PLAN.md`. Anything not yet built is marked "coming soon". Product screenshots are added only after the interfaces have been reviewed and approved (plan section 34.1).

## Ownership

&copy; 2026 Lattice AI LLC. Every page's footer carries the same notice.

## Deployment

Pushing to `main` deploys through GitHub Pages once Pages is enabled for the repository (branch `main`, folder `/`) and DNS for `mymorningnews.ai` points at GitHub Pages.

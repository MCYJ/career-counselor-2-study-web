# Career Counselor Level 2 · 한국어 500제

An independent study-app information site by RushLabs, hosted on GitHub Pages.

- 한국어: https://mcyj.github.io/career-counselor-2-study-web/ko/
- English: https://mcyj.github.io/career-counselor-2-study-web/en/

The app is **preparing for launch**. Download links stay disabled until public store availability is verified. Questions and written practice cases are in Korean; translating this website does not translate the app’s question bank.

## Content and privacy

The site describes a planned paid-upfront study app: 500 original multiple-choice questions, explanations for every option, timed practice using the same question bank, and four fictional written-practice cases. It does not reproduce official exam questions or third-party articles/images. The study-flow graphic is a web illustration, not an app screenshot.

No analytics, external fonts, tracking scripts or enquiry forms are included. See the [GitHub privacy statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement) for hosting information. App-local records and user-managed backups are described on the privacy page.

## Develop

Node.js is sufficient; no dependency installation is required.

```sh
npm test
npm run preview
```

Preview: `http://127.0.0.1:4187/career-counselor-2-study-web/ko/`

- `content/site.mjs`: Korean/English copy and site settings
- `styles.css`: responsive design, keyboard focus and reduced-motion styles
- `scripts/build.mjs`: static pages, metadata, sitemap and 404
- `scripts/check.mjs`: routes, links, identity, metadata and disabled download checks
- `scripts/serve.mjs`: localhost Project Pages preview
- `assets/app-icon.png`: RushLabs’ existing subject icon

## Publish

The Pages workflow builds and checks the site, uploads only `dist`, and deploys through the `github-pages` environment. Its base path must match the repository name. `PUBLIC_SITE_URL` may override the configured HTTPS site URL when the hostname or path changes.

This coming-soon site remains `noindex` and blocks crawling in `robots.txt`. Publishing the website does not publish the mobile app. Update download links, screenshots and indexing only when the corresponding public app and product features have been verified.

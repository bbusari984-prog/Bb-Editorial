# BB Editorial Services — Non-Fiction Editing Website

A single-page, SEO/AEO/GEO-optimized website for **BB Editorial Services**, Barakat Busari's freelance editing business specializing exclusively in **non-fiction books**, built to be hosted for free with **GitHub Pages** and linked from an Upwork profile.

## 🎨 Design

- **Brand palette:** Bordeaux (`#5c0f1e`, `#3d0a14`) mixed with warm cream (`#f7f0e3`, `#fbf6ea`) and a gold accent (`#c8a15c`) — a literary, editorial, high-end feel.
- **Typography:** Playfair Display (serif, headings) paired with Jost (sans-serif, body) via Google Fonts.
- Fully responsive layout with a mobile slide-out navigation drawer, animated hover states, accordion FAQ, and a dedicated contact block.
- Single self-contained `index.html` file — all CSS and JavaScript are inlined, so there is nothing else to configure.

## 📄 Files in this repository

| File | Purpose |
|---|---|
| `index.html` | The full website (structure, styling, and interactivity in one file). |
| `sitemap.xml` | XML sitemap listing the page's sections for search engine crawlers. |
| `robots.txt` | Crawler rules pointing search engines and AI crawlers to the sitemap. |
| `llms.txt` | AI/answer-engine-readable summary of the business, services, and pricing. |
| `README.md` | This file. |

Your photo is embedded directly inside `index.html` as base64 (no separate image file needed) — this avoids the broken-image issue that happens when an image file gets left out of an upload.

## 🔍 SEO / AEO / GEO Features

This site is built with **three layers of discoverability** in mind:

- **SEO (Search Engine Optimization):** semantic HTML5, descriptive `<title>` and `<meta name="description">`, keyword-relevant headings, canonical URL tag, Open Graph and Twitter Card meta tags, and a submitted `sitemap.xml` + `robots.txt`.
- **AEO (Answer Engine Optimization):** an on-page, visually accordion-based **FAQ section** is mirrored in machine-readable `FAQPage` JSON-LD structured data, so voice assistants and AI answer engines (Google AI Overviews, Bing Copilot, ChatGPT browsing, Perplexity, etc.) can extract direct question-and-answer pairs.
- **GEO (Generative Engine Optimization):** `ProfessionalService` and `Person` JSON-LD schema, plus `llms.txt`, describe the service type, pricing, and contact details in a structured format that generative AI systems can cite directly when recommending a non-fiction editor.

## 🚀 How to publish with GitHub Pages

1. Create a new **public** GitHub repository.
2. Upload all files in this folder to the root of that repository (drag-and-drop works fine on github.com, or use `git add . && git commit -m "Update site" && git push`).
3. In the repository, go to **Settings → Pages**.
4. Under **Source**, choose the `main` branch and `/ (root)` folder, then click **Save**.
5. GitHub will publish your site at either:
   - `https://<your-username>.github.io/<repository-name>/` (project repo), or
   - `https://<your-username>.github.io/` (if the repo is named exactly `<your-username>.github.io`).
6. Wait 1–2 minutes, then visit the URL to confirm it's live.

Your current live URL is: `https://bbusari984-prog.github.io/Oluwabunmi-/`

### If you change the URL

If you ever move to a different GitHub username or repository name, search-and-replace every instance of the URL above across `index.html`, `sitemap.xml`, `robots.txt`, and `llms.txt`.

Optional but recommended: add a real `assets/og-cover.jpg` image (1200×630px) to the repository and update the `og:image` / `twitter:image` tags in `index.html` so link previews on WhatsApp, LinkedIn, and social media show a proper cover image instead of a broken link.

## ✏️ Customizing content

Everything is in `index.html`. Useful anchors to search for and edit directly:

- **Hero headline & subtext** — inside `<section class="hero">`
- **Services & pricing** — inside `<section id="services">` (`.service-card` blocks)
- **About / bio / stats / non-fiction categories** — inside `<section id="about">`
- **Process steps** — inside `<section id="process">`
- **Samples** — inside `<section id="samples">`; each `.sample-card` links out to an Upwork portfolio project. Replace the placeholder titles/descriptions with the real project names once you share them.
- **Testimonials** — inside `<section id="testimonials">`; **currently placeholder text** — replace with your exact Upwork review quotes (client name/role can stay generic like "Upwork Client" if you prefer not to publish real names).
- **FAQ** — inside `<section id="faq">`; each `<details>` block is one question. Keep the matching `FAQPage` JSON-LD block near the top of the file in sync with any wording changes.
- **Contact details** — WhatsApp and email appear in the `<section id="contact">` block and in the footer.

## ⚠️ Still needs your input

- **Samples:** the four sample cards currently link to your Upwork portfolio items but use generic titles ("Sample Project 1", etc.). Send a one-line title/description for each project and they'll be updated to something more descriptive.

## 📞 Contact details used on this site

- **WhatsApp:** +234 813 164 2111
- **Email:** busaribaraka1@gmail.com
- **Upwork:** https://www.upwork.com/freelancers/busarib

## 🛠 Tech stack

Pure HTML5, CSS3, and vanilla JavaScript — no build step, no dependencies, no frameworks. Works on any static host (GitHub Pages, Netlify, Vercel, Cloudflare Pages) with zero configuration.

## 📈 Recommended next steps

- Submit the sitemap URL to [Google Search Console](https://search.google.com/search-console) and [Bing Webmaster Tools](https://www.bing.com/webmasters) after publishing.
- Replace placeholder testimonials and sample descriptions with real content (see above).
- Add a custom domain (optional) via **Settings → Pages → Custom domain** in your GitHub repository, and update the `canonical`, `og:url`, and sitemap URLs to match.

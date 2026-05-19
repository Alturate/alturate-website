# alturate.com

Marketing site for **Alturate** — a senior-led Microsoft Dynamics 365 Finance & Operations specialist practice. We help mid-market manufacturers and distributors migrate to Microsoft Fabric, prepare their ERP data for Copilot, and ship working AI agents in Copilot Studio.

**Live site:** [www.alturate.com](https://www.alturate.com)

---

## What's in this repo

A static site, no build step. Just HTML + inline CSS. Hosted as static files.

```
index.html         Homepage — hero, problem, offers, ICP, CTA
services.html      Four offers in detail (Assessment, Fabric, Agent Pilot, Managed)
assessment.html    18-question Copilot Readiness Assessment (interactive)
about.html         Founder story + values
contact.html       Booking form + sidebar
sitemap.xml        For Google/Bing indexing
robots.txt         Crawler allowlist + sitemap pointer
```

## The offer ladder

1. **Free Readiness Assessment** — 18 questions, instant score (assessment.html)
2. **D365 F&O Readiness Assessment** — $15K fixed, 3 weeks, written roadmap
3. **Fabric Reporting Modernization** — $35–95K, 6–10 weeks
4. **Copilot Studio Agent Pilot** — $40–95K, 8–12 weeks
5. **Managed Services** — monthly retainer

## Tech stack

- Pure HTML + inline CSS (Plus Jakarta Sans, gold/navy palette)
- No framework, no build, no JS dependencies (assessment.html has a small inline JS quiz engine)
- Embedded base64 logo/favicon (no external image dependencies)
- SEO: schema.org JSON-LD, Open Graph, Twitter cards, sitemap, robots
- Mobile-responsive

## Local preview

Just open `index.html` in a browser. No server needed for the marketing pages. The assessment uses inline JS only.

For local hosting with proper URLs:
```bash
python3 -m http.server 8000
# Then visit http://localhost:8000
```

## Deployment

Any static host works — Cloudflare Pages, Netlify, Vercel, GitHub Pages, or a plain S3 bucket. Recommended: Cloudflare Pages (free, fast CDN, native GitHub integration).

## TODO before public launch

- [ ] Replace `https://www.linkedin.com/in/your-handle` with real LinkedIn URL (4 places)
- [ ] Add founder photo to about.html
- [ ] Wire up the contact form (currently inert — needs Formspree, HubSpot Forms, or backend)
- [ ] Wire up assessment.html email delivery (form captures email but needs a backend or Zapier hook)
- [ ] Set up email forwarding for `hello@alturate.com`
- [ ] Submit sitemap to Google Search Console + Bing Webmaster Tools
- [ ] Add a real `og:image` (currently absent — LinkedIn previews will be plain text)

## Entity

© Alturate LLP (India). All rights reserved.

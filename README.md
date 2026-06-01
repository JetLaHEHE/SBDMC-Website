# SBDMC — Subic Bay Development & Management Corporation

Corporate website for SBDMC (Subic Bay Gateway Park), built with [Astro](https://astro.build/) and [Tailwind CSS](https://tailwindcss.com/).

## Features

- **16 static pages** — Home, About, FAQ, Jobs, Gallery, Contact, and more
- **Sticky glass-morphism header** with dropdown navigation and mobile toggle
- **Scroll-triggered animations** via AOS (Animate on Scroll)
- **Back-to-top button**, hover lift effects, gradient accents
- **Content managed via Decap CMS** (Netlify CMS) — edit hero, news, FAQ, jobs, and contact data through a browser UI
- **Fully static** — no server runtime, deploys anywhere

## Tech Stack

| Tool | Purpose |
|------|---------|
| [Astro 5](https://astro.build/) | Static site framework |
| [Tailwind CSS 3](https://tailwindcss.com/) | Utility-first styling |
| [AOS](https://michalsnik.github.io/aos/) | Scroll animations |
| [Decap CMS](https://decapcms.org/) | Git-backed content management |

## Content Management

The admin panel is available at `/admin` (requires Netlify Identity + Git Gateway).

Editable collections:
- **Home Hero** — headline, stats, CTAs, section titles
- **News Links** — news article cards
- **FAQ** — categorized Q&A items
- **Job Listings** — open/closed positions
- **Contact Info** — address, phone, email, hours

For local CMS development:
```bash
npx decap-server
```
Then visit `http://localhost:4321/admin`.

## Development

```bash
npm install
npm run dev      # starts dev server at localhost:4321
npm run build    # builds static output to dist/
npm run preview  # preview the production build
```

## Deployment

Push to GitHub → connect to Netlify → enable Identity + Git Gateway → invite collaborators.

Build settings (auto-detected via `netlify.toml`):
- Build command: `npm run build`
- Publish directory: `dist`

## License

All rights reserved. © SBDMC

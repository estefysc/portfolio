# >_ portfolio

My personal portfolio site.

Built with a brutalist aesthetic: monospace typography, neon orange on black, zero border-radius, terminal-inspired UI.

## Tech Stack

- [Astro](https://astro.build/) — static site generator
- [Tailwind CSS v4](https://tailwindcss.com/) — utility-first styling
- [Cloudflare Pages](https://pages.cloudflare.com/) — hosting and deployment

## Local Development

```bash
npm install
npm run dev
```

Site runs at `http://localhost:4321`.

## Build

```bash
npm run build
```

Output goes to `dist/`.

## Project Structure

```
src/
├── components/
│   ├── Nav.astro          # navigation with mobile hamburger menu
│   ├── Section.astro      # reusable section wrapper
│   └── ProjectCard.astro  # project card component
├── layouts/
│   └── Layout.astro       # base HTML layout with SEO meta tags
├── pages/
│   └── index.astro        # single-page site with all sections
└── styles/
    └── global.css         # tailwind theme and brutalist base styles
public/
├── _headers               # cloudflare pages security headers (CSP, etc.)
├── favicon.svg            # >_ terminal prompt icon
└── resume.pdf             # downloadable resume
```

## Features

- Typing animation on hero intro
- Native HTML `<details>` accordions for skills and experience (zero JS)
- Mobile-responsive hamburger menu
- Security headers: CSP, X-Frame-Options, Referrer-Policy
- Open Graph and Twitter Card meta tags
- Console easter egg for the curious

## License

All rights reserved.

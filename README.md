# blog.voltii

Source for [voltii.blog](https://voltii.blog) — the build journal for a 1973 BMW 2002tii EV conversion.

Built with [Astro](https://astro.build), deployed on [Cloudflare Pages](https://pages.cloudflare.com), static output, no server, no database.

## Structure

- `src/content/posts/*.md` — journal entries. Each needs frontmatter:
  ```yaml
  ---
  title: "Post title"
  description: "One-line summary (optional, shown in listing)"
  date: 2026-08-29
  heroImage: "/images/whatever.jpg"   # optional
  tags: ["gearbox", "brakes"]          # optional
  ---
  ```
- `public/images/` — drop photos here, reference as `/images/filename.jpg` in posts.
- `src/pages/about.astro` — the car's backstory (static page).
- `src/pages/technical.astro` — living technical spec summary (static page).
- `src/layouts/` — page templates.

## Local development

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
```

Outputs static files to `dist/`, which Cloudflare Pages serves directly.

## Deploy

Push to `main` — Cloudflare Pages is connected to this repo and rebuilds
automatically on every push. Build command: `npm run build`. Output directory: `dist`.

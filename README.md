# harshkhatore.github.io

Personal portfolio website for **Harsh Khatore** — Software Engineer.

Built with a **futuristic techno** aesthetic: dark backgrounds, neon accents, grid patterns, terminal-style UI, and smooth animations.

## Tech Stack

- **[Astro](https://astro.build)** — Static site generator (fast, component-based, easy to maintain)
- **[TailwindCSS](https://tailwindcss.com)** — Utility-first CSS framework
- **TypeScript** — Type-safe development
- **GitHub Pages** — Hosting via GitHub Actions

## Project Structure

```
src/
├── components/
│   ├── Navbar.astro      # Navigation bar with mobile menu
│   ├── Hero.astro        # Hero section with animated particles
│   ├── About.astro       # About section with terminal UI
│   ├── Skills.astro      # Skills & tech stack grid
│   ├── Projects.astro    # Projects showcase cards
│   ├── Contact.astro     # Contact section with social links
│   └── Footer.astro      # Footer
├── layouts/
│   └── Layout.astro      # Base layout with global styles
└── pages/
    └── index.astro       # Main page
```

## Commands

| Command           | Action                                     |
| :---------------- | :----------------------------------------- |
| `npm install`     | Install dependencies                       |
| `npm run dev`     | Start dev server at `localhost:4321`       |
| `npm run build`   | Build production site to `./dist/`         |
| `npm run preview` | Preview build locally before deploying     |

## Deployment

Deployment is automated via GitHub Actions. Every push to `main` triggers a build and deploy to GitHub Pages.

## Customization

- **Content**: Edit component files in `src/components/` to update text, links, and sections
- **Theme colors**: Modify `tailwind.config.mjs` to change the neon color palette
- **Add pages**: Create new `.astro` files in `src/pages/`

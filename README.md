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
│   ├── Experience.astro  # Experience & Patents section
│   ├── BeyondCode.astro  # Beyond Code section
│   ├── Contact.astro     # Contact section with social links
│   └── Footer.astro      # Footer
├── layouts/
│   └── Layout.astro      # Base layout with global styles
└── pages/
    └── index.astro       # Main page
```

## Getting Started

### Prerequisites

- **Node.js** (v18 or higher) — [Download](https://nodejs.org/)
- **npm** (comes with Node.js)
- **Git** — [Download](https://git-scm.com/)

### Installation & Local Development

1. **Clone the repository**:
   ```bash
   git clone https://github.com/HarshKhatore/harshkhatore.github.io.git
   cd harshkhatore.github.io
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Start the development server**:
   ```bash
   npm run dev
   ```
   The site will be available at `http://localhost:4322` (or the next available port if 4322 is in use).

4. **Open in browser**:
   - Navigate to `http://localhost:4322`
   - Changes to files will hot-reload automatically
   - Open DevTools (F12) to inspect and debug

### Building for Production

1. **Build the static site**:
   ```bash
   npm run build
   ```
   This generates optimized files in the `./dist/` directory.

2. **Preview the production build locally**:
   ```bash
   npm run preview
   ```
   This serves the production build at `http://localhost:3000` so you can test before deploying.

3. **Verify the build**:
   - Check that `./dist/` contains all necessary files
   - Test all links and interactive elements
   - Ensure styling and animations work correctly

## Commands Reference

| Command           | Action                                     |
| :---------------- | :----------------------------------------- |
| `npm install`     | Install dependencies                       |
| `npm run dev`     | Start dev server at `http://localhost:4322` |
| `npm run build`   | Build production site to `./dist/`         |
| `npm run preview` | Preview production build locally            |

## Branching Strategy

This project follows a **component-based branching model** to keep changes organized and easy to review. All work should be done on feature branches before merging to `main`.

### Branch Naming Convention

Use the following prefixes based on the type of change:

| Prefix | Purpose | Example |
| :--- | :--- | :--- |
| `ui/` | Cosmetic/styling changes (colors, animations, layout tweaks) | `ui/neon-glow-effect`, `ui/navbar-mobile-menu` |
| `content/` | Content updates (text, descriptions, links) | `content/update-about-section`, `content/add-experience` |
| `feature/` | New features or major component additions | `feature/dark-mode-toggle`, `feature/blog-section` |
| `fix/` | Bug fixes | `fix/navbar-scroll-issue`, `fix/mobile-responsive` |
| `refactor/` | Code refactoring without changing functionality | `refactor/component-structure`, `refactor/tailwind-cleanup` |
| `docs/` | Documentation updates | `docs/update-readme`, `docs/add-contributing-guide` |

### Component-Specific Branches

For changes to specific components, use the component name in the branch:

- **Experience updates**: `content/experience-*` (e.g., `content/experience-add-patents`)
- **About section**: `content/about-*` (e.g., `content/about-update-bio`)
- **Beyond Code section**: `content/beyond-code-*` (e.g., `content/beyond-code-add-hobby`)
- **UI styling**: `ui/component-name-*` (e.g., `ui/experience-card-styling`)

### Workflow

1. **Create a branch** from `main`:
   ```bash
   git checkout -b ui/navbar-styling
   ```

2. **Make your changes** and commit with clear messages:
   ```bash
   git commit -m "Update navbar hover effects and spacing"
   ```

3. **Push to remote**:
   ```bash
   git push origin ui/navbar-styling
   ```

4. **Create a Pull Request** on GitHub and describe your changes

5. **Merge to `main`** once reviewed:
   ```bash
   git checkout main
   git pull origin main
   git merge ui/navbar-styling
   git push origin main
   ```

6. **Delete the branch** after merging:
   ```bash
   git branch -d ui/navbar-styling
   git push origin --delete ui/navbar-styling
   ```

### Commit Message Guidelines

- Use imperative mood: "Add feature" not "Added feature"
- Be specific: `content/experience-add-patents` → "Add patent entries to Experience section"
- Keep it concise but descriptive

## Deployment

Deployment is automated via GitHub Actions. Every push to `main` triggers a build and deploy to GitHub Pages.

## Customization

- **Content**: Edit component files in `src/components/` to update text, links, and sections
- **Theme colors**: Modify `tailwind.config.mjs` to change the neon color palette
- **Add pages**: Create new `.astro` files in `src/pages/`

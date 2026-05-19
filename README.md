# Personal Website

Personal portfolio and blog for Muhammad Iqbal, built with Next.js, Tailwind CSS, `shadcn/ui`, and Magic UI.

This codebase is configured as a static export and can be deployed to GitHub Pages.

## Stack

- Next.js 16
- React 19
- TypeScript
- Tailwind CSS v4
- `shadcn/ui`
- Content Collections for blog content

## Project Structure

- [src/data/resume.tsx](/Users/efishery/Documents/workspace/portfolio/src/data/resume.tsx:1)
  Main content source for profile data, work experience, education, capabilities, tech stack, and contact links.
- [content/](/Users/efishery/Documents/workspace/portfolio/content)
  MDX blog posts.
- [src/app/](/Users/efishery/Documents/workspace/portfolio/src/app)
  App Router pages and layouts.
- [public/](/Users/efishery/Documents/workspace/portfolio/public)
  Static assets such as profile photo, company logos, and tech stack logos.
- [.github/workflows/deploy-pages.yml](/Users/efishery/Documents/workspace/portfolio/.github/workflows/deploy-pages.yml:1)
  GitHub Pages deployment workflow.

## Local Development

1. Install dependencies:

```bash
pnpm install
```

2. Start the dev server:

```bash
pnpm dev
```

3. Open `http://localhost:3000`

## Content Updates

Most site content can be updated by editing:

```bash
src/data/resume.tsx
```

Blog posts live in:

```bash
content/*.mdx
```

## Static Build

To verify the static export locally:

```bash
NEXT_PUBLIC_SITE_URL=https://iqbal-codes.github.io pnpm build:static
```

For a GitHub Pages project site, set:

```bash
NEXT_PUBLIC_SITE_URL=https://<username>.github.io/<repo-name>
NEXT_PUBLIC_BASE_PATH=/<repo-name>
```

For a GitHub Pages user site, set:

```bash
NEXT_PUBLIC_SITE_URL=https://<username>.github.io
NEXT_PUBLIC_BASE_PATH=
```

## GitHub Pages Deployment

This repo includes a GitHub Actions workflow for static deployment.

To use it:

1. Push the repo to GitHub.
2. Open `Settings -> Pages`.
3. Set `Source` to `GitHub Actions`.
4. Update the environment values in `.github/workflows/deploy-pages.yml` if your Pages URL changes.

## Notes

- The site uses static export mode via `next.config.mjs`.
- Dynamic Open Graph image routes were removed to keep GitHub Pages deployment stable.
- Generated blog content is built at compile time.

## License

MIT. See [LICENSE](/Users/efishery/Documents/workspace/portfolio/LICENSE:1).

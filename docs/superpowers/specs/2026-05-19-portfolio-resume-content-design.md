# Portfolio Resume Content Design

## Goal

Update the portfolio website so its visible content matches Muhammad Iqbal's resume, without redesigning the site structure or animation system.

## Scope

- Replace hero copy, about copy, work experience, skills, education, contact details, and social links with resume-backed content.
- Replace the current hero photo with the provided portrait.
- Remove the blog entry from navigation.
- Remove the projects section from the homepage for now.
- Keep the existing visual design, layout, and section ordering where practical.

## Content Decisions

### Hero

- Name: Muhammad Iqbal
- Location: Bandung, Indonesia
- Intro should present him as a Senior Software Engineer with 7+ years of experience.
- Avatar should use the provided replacement photo.

### About

- Rewrite the current summary into concise website copy derived from the resume summary.
- Emphasize frontend depth, fullstack delivery, maintainability, testing, and AI-assisted engineering workflows.

### Work Experience

Use these resume-backed roles only:

1. PT Kaldu Sari Nabati Indonesia (KSNI) — Senior Frontend Engineer
2. eFishery — Frontend Engineer
3. Pertamedika IHC (Contract) — Lead Frontend Engineer
4. Virtual Spirit — Frontend Engineer
5. Komers — Frontend Engineer

Each role should be rewritten into readable portfolio copy rather than pasted raw as CV bullets.

### Skills

Replace current skills with resume-backed technologies and competencies, prioritizing:

- React
- Next.js
- TypeScript
- React Native
- Expo
- Node.js
- tRPC
- PostgreSQL
- Jest
- Testing Library
- Turborepo
- Monorepo Architecture
- Micro-Frontend
- GraphQL
- AI-Assisted Development

Icons should be shown where already available. Skills without matching icons can remain text-only pills.

### Education

- Keep only Bandung State Polytechnic (POLBAN)
- Degree: Diploma 3 - Software Engineering
- Years: 2015 - 2018

### Navigation and Contact

- Remove Blog from navbar.
- Keep Home in navbar.
- Social/contact links should include:
  - LinkedIn
  - Instagram
  - Email
- Contact section copy should no longer reference Twitter/X and should instead invite contact through email or LinkedIn/Instagram.

## Template Adjustments

- Remove `ProjectsSection` from the homepage render.
- Keep commented hackathon section untouched unless needed.
- Extend icons set with an Instagram icon so the contact/navbar data remains consistent.

## Risks

- The existing data file is a large template-driven object, so edits must preserve the shape expected by the UI.
- The user has an existing uncommitted formatting-only change in `src/app/page.tsx`; implementation should avoid overwriting unrelated edits.

## Verification

- Run lint after the content update.
- Confirm the new avatar asset is referenced correctly.
- Confirm the homepage no longer renders the projects section and the navbar no longer includes Blog.

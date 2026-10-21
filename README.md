# Ilham Insani — Career Website

A responsive bilingual (English / Bahasa Indonesia) personal career website with an executive dark-navy visual system, built with Next.js App Router, React, TypeScript, and custom CSS.

## Features
- Responsive desktop, tablet, and mobile layouts
- Working English / Bahasa Indonesia toggle
- About, experience, research, capabilities, recognition, and contact sections
- Accessible navigation and reduced-motion support
- SEO metadata and Open Graph basics
- No database or environment variables required

## Requirements
- Node.js 20.9 or newer
- npm

## Run locally

1. Extract the ZIP and open a terminal in the `ilham-career-website` directory.
2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the development server:

   ```bash
   npm run dev
   ```

4. Open http://localhost:3000

## Production build

```bash
npm run build
npm run start
```

## Deploy to Vercel

1. Create a GitHub repository and push this folder to it.
2. Sign in to Vercel and choose **Add New → Project**.
3. Import the GitHub repository. Vercel should detect Next.js automatically.
4. Keep the default build settings and select **Deploy**.
5. After deployment, add a custom domain in the Vercel project settings if you own one.

## Before publishing — review these items

1. **CV download:** No CV file is bundled. If you want a public download, add a reviewed PDF at `public/Ilham-Insani-CV.pdf`, then add a link to `/Ilham-Insani-CV.pdf` in `app/page.tsx`.
2. **Research details:** Confirm each project's title, role, methods, and reported results against your final paper or project record. The 0.12 V/cell figure is presented as a reported project result, not as a performance guarantee.
3. **AI work:** The page describes AI-related evaluation workflows without claiming AI-expert status or naming a platform as an employer.
4. **Experience:** Check dates and role descriptions for accuracy before making the website public.
5. **SEO domain:** In `app/layout.tsx`, replace `https://example.com` in `metadataBase` with your deployed domain.
6. **Fonts:** Google Fonts are loaded via CSS. If you prefer no third-party font requests, remove the `@import` and use system font fallbacks.

## Main files
- `app/page.tsx` — page content, language toggle, sections, and links
- `app/globals.css` — visual design and responsive breakpoints
- `app/layout.tsx` — metadata and root layout
- `package.json` — dependencies and commands

# Web Application

Main Next.js application serving as the portfolio landing page and navigation hub.

## Purpose

- Landing page with project overview
- Navigation to demo applications
- About section and contact information
- Responsive design showcasing UI/UX skills

## Tech Stack

- Next.js 14+ (App Router)
- TypeScript
- Tailwind CSS
- Shared UI components from `@repo/ui`

## Development

```bash
# From root directory
pnpm dev --filter=web

# Or from this directory
pnpm dev
```

The app will be available at `http://localhost:3000`

## Build

```bash
pnpm build
```

## Structure

```
web/
├── app/              # Next.js App Router pages
├── components/       # App-specific components
├── public/          # Static assets
├── styles/          # Global styles
└── package.json
```

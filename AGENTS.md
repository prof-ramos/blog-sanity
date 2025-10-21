# Agent Guidelines for Next.js Blog with Sanity CMS

## Commands

- **Build**: `npm run build` (includes Sanity manifest extraction)
- **Dev**: `npm run dev` (uses Turbopack)
- **Lint**: `npm run lint` (ESLint with Next.js config)
- **Format**: `npm run format` (Prettier)
- **Type Check**: `npm run type-check` (TypeScript)
- **Fix All**: `npm run lint:fix` (format + lint --fix)

## Code Style

- **Formatting**: Prettier with no semicolons, single quotes
- **Imports**: Sorted with `simple-import-sort` (external first, then relative)
- **Types**: TypeScript with `strict: false`, `strictNullChecks: false`
- **Components**: PascalCase, functional with typed props
- **Naming**: camelCase for variables/functions, PascalCase for types
- **Styling**: Tailwind CSS classes, responsive design
- **Error Handling**: Throw descriptive Error objects
- **JSX**: Multi-line props on separate lines

## Architecture

- **Framework**: Next.js 15 with App Router
- **CMS**: Sanity v4 with GROQ queries
- **Styling**: Tailwind CSS v4
- **Components**: Located in `/components`, imported relatively
- **Pages**: Mix of App Router (`/app`) and Pages Router (`/pages`)
- **Data**: Sanity client in `/lib`, queries in `sanity.queries.ts`

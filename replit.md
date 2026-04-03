# Workspace

## Overview

pnpm workspace monorepo using TypeScript. Each package manages its own dependencies.

## Stack

- **Monorepo tool**: pnpm workspaces
- **Node.js version**: 24
- **Package manager**: pnpm
- **TypeScript version**: 5.9
- **API framework**: Express 5
- **Database**: PostgreSQL + Drizzle ORM
- **Validation**: Zod (`zod/v4`), `drizzle-zod`
- **API codegen**: Orval (from OpenAPI spec)
- **Build**: esbuild (CJS bundle)

## Key Commands

- `pnpm run typecheck` — full typecheck across all packages
- `pnpm run build` — typecheck + build all packages
- `pnpm --filter @workspace/api-spec run codegen` — regenerate API hooks and Zod schemas from OpenAPI spec
- `pnpm --filter @workspace/db run push` — push DB schema changes (dev only)
- `pnpm --filter @workspace/api-server run dev` — run API server locally

See the `pnpm-workspace` skill for workspace structure, TypeScript setup, and package details.

## Artifacts

### MD Resin Art (`artifacts/md-resin`)
- **Type**: react-vite (presentation-first, no backend)
- **Preview path**: `/`
- **Description**: Elegant landing page for MD Resin, a handmade resin art brand from Neyveli, India
- **Features**: Hero section with logo, product categories (keychains/frames/stationery), brand story, how-to-order, gallery, contact/footer
- **Design**: Warm golden-beige, champagne, cream, teal accents, glassmorphism cards, framer-motion animations, Cormorant Garamond serif font
- **Assets**: Logo at `artifacts/md-resin/public/md-resin-logo.png`, AI-generated product/gallery images in `/public/images/`
- **Contact**: WhatsApp + Instagram (@md_resinart_neyveli)

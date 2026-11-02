# Project Instructions

## Project

This is a Hebrew-language equipment lending app built with React, TypeScript, Vite, Tailwind CSS, and Supabase. Users browse available items and submit borrowing requests; the admin screen manages request and item statuses.

## Commands

- `npm run dev` starts the Vite development server.
- `npm run build` runs the production build.
- `npm run lint` runs ESLint.
- `npm run typecheck` runs the application TypeScript check.

## Codebase Conventions

- Application code lives in `src/`; use the `@/` alias for imports from `src/`.
- Keep the existing React function-component and TypeScript patterns.
- Use Tailwind utility classes for styling and `lucide-react` for icons.
- Keep user-facing copy in Hebrew, matching the existing right-to-left interface.
- Supabase client setup and shared row types live in `src/lib/supabase.ts`.
- Database schema changes belong in `supabase/migrations/`; keep client queries and TypeScript types consistent with the schema.
- Configure Supabase with `VITE_SUPABASE_URL` and `VITE_SUPABASE_ANON_KEY`. Never commit credentials or secrets.

## Structure

- `src/App.tsx` coordinates the home, item detail, and admin views.
- `src/pages/` contains the main screens.
- `src/components/` contains shared UI components.
- `supabase/migrations/` contains database migrations.
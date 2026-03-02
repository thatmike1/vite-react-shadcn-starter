# vite-react-shadcn-starter

Opinionated starter template for building apps with Vite, React, and shadcn/ui.

## Tech Stack

| Category | Tech |
|---|---|
| **Framework** | React 19 + TypeScript |
| **Build** | Vite 6 (SWC) |
| **Styling** | Tailwind CSS v4 |
| **Components** | shadcn/ui (New York style) |
| **Icons** | Lucide React |
| **Routing** | React Router v7 |
| **Data Fetching** | TanStack React Query v5 |
| **Forms** | React Hook Form + Zod v4 |
| **Toasts** | Sonner |

## What's Included

- React Query provider
- React Router with layout pattern
- Path aliases (`@/` -> `src/`)
- ESLint with `no-explicit-any` set to error
- Base shadcn/ui components: Button, Input, Label, Card, Sonner

## Getting Started

```bash
# clone
git clone https://github.com/thatmike1/vite-react-shadcn-starter.git my-app
cd my-app

# install
npm install

# run
npm run dev
```

## Project Structure

```
src/
  components/ui/     # shadcn/ui components
  hooks/             # custom hooks
  lib/               # query client, utils (cn)
  pages/             # layout
  App.tsx
  main.tsx
```

## Adding shadcn/ui Components

```bash
npx shadcn@latest add [component-name]
```

## Conventions

- Kebab-case file names (`use-auth.ts`, not `useAuth.ts`)
- `.ts` for hooks/utils, `.tsx` only when returning JSX
- No `any` types (eslint will error)

## Looking for Supabase?

Check out [vite-react-supabase-starter](https://github.com/thatmike1/vite-react-supabase-starter) which adds Supabase auth, protected routes, and a login page on top of this template.

## License

MIT

# Project Structure

```text
yeabsira-portfolio/
├── app/                    # Next.js App Router
│   ├── (public)/           # Public-facing routes group
│   │   ├── page.tsx        # Home page (Bento Grid)
│   │   ├── projects/       # Project detail pages
│   │   │   └── [slug]/
│   │   │       └── page.tsx
│   │   └── layout.tsx
│   ├── (admin)/            # Admin dashboard routes group
│   │   ├── admin/
│   │   │   ├── projects/
│   │   │   └── messages/
│   │   └── layout.tsx
│   ├── api/                # Route Handlers
│   │   ├── projects/
│   │   ├── contact/
│   │   └── auth/
│   ├── layout.tsx          # Root layout
│   ├── loading.tsx         # Global loading state
│   ├── error.tsx           # Global error boundary
│   └── globals.css         # Global Tailwind styles
├── components/             # React components
│   ├── bento/              # Bento grid specific components
│   │   ├── Grid.tsx
│   │   ├── Cell.tsx
│   │   └── ProjectCard.tsx
│   ├── ui/                 # Reusable UI primitives (Radix-based)
│   │   ├── Button.tsx
│   │   ├── Input.tsx
│   │   └── Modal.tsx
│   ├── layout/             # Layout-specific components
│   │   ├── FloatingDock.tsx
│   │   ├── Footer.tsx
│   │   └── MobileNav.tsx
│   ├── motion/             # Animation wrappers
│   │   ├── Reveal.tsx
│   │   └── SmoothScroll.tsx (Lenis setup)
│   └── shared/             # General shared components
├── lib/                    # Utilities and shared logic
│   ├── gsap.ts             # GSAP configuration and plugins
│   ├── prisma.ts           # Prisma client instance
│   ├── utils.ts            # Tailwind-merge and clsx helpers
│   └── supabase.ts         # Supabase client
├── hooks/                  # Custom React hooks
│   ├── use-scroll.ts       # Scroll position tracking
│   └── use-store.ts        # Zustand store definitions
├── types/                  # TypeScript type definitions
│   ├── project.ts
│   └── index.ts
├── prisma/                 # Prisma schema and migrations
│   └── schema.prisma
├── public/                 # Static assets
│   ├── fonts/              # Custom fonts (Syne, JetBrains Mono)
│   ├── images/
│   └── videos/
├── .github/                # CI/CD workflows
└── tailwind.config.ts      # Tailwind configuration
```

## File Naming Conventions
- **Components**: PascalCase (e.g., `ProjectCard.tsx`)
- **Hooks**: camelCase with `use-` prefix (e.g., `use-scroll.ts`)
- **Utilities**: camelCase (e.g., `gsap.ts`)
- **Routes**: lowercase with hyphens (e.g., `projects/[slug]/`)
- **Styles**: lowercase with hyphens (e.g., `globals.css`)

## Component Architecture
- **Server Components**: Used for data fetching in `app/` and static sections.
- **Client Components**: Used for interactive elements like the Bento cells, Floating Dock, and any component requiring GSAP/Framer Motion or state hooks. Marked with `'use client'`.

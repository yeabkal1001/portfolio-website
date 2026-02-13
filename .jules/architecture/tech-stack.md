# Tech Stack

## Frontend
- **Framework**: Next.js 14 (App Router)
- **Language**: TypeScript
- **Styling**: Tailwind CSS + Class Variance Authority (CVA)
- **UI Components**: Radix UI (Accessible primitives)
- **Animation**:
  - **GSAP**: For complex scroll-triggered timelines and coordinate-based animations.
  - **Framer Motion**: For declarative UI transitions and layout animations.
  - **Lenis Scroll**: For high-performance momentum-based smooth scrolling.
- **State Management**: Zustand (Lightweight global state)
- **Icons**: Lucide React
- **Forms**: React Hook Form + Zod (Schema validation)

## Backend
- **Runtime**: Node.js 20+
- **Framework**: Next.js API Routes (Route Handlers)
- **Language**: TypeScript
- **API Style**: REST

## Database
- **Database**: PostgreSQL
- **ORM**: Prisma
- **Hosting**: Supabase (Database, Auth, and Storage)

## Authentication
- **Solution**: Supabase Auth / NextAuth.js
- **Methods**: Magic Links + OAuth (GitHub/LinkedIn) for Admin access.

## Storage
- **Images/Assets**: Supabase Storage
- **CDN**: Vercel Edge Network

## Deployment
- **Platform**: Vercel
- **CI/CD**: GitHub Actions
- **Environment**: Preview + Production

## Monitoring
- **Analytics**: Vercel Analytics
- **Error Tracking**: Sentry
- **Performance**: Lighthouse CI (Integrated into GitHub Actions)

## Rationale

### Why Next.js 14?
Next.js 14 provides the best-in-class performance with Server Components, reducing the bundle size sent to the client. This is crucial for meeting the Lighthouse 90+ performance target. The App Router allows for nested layouts and simplified data fetching.

### Why GSAP + Framer Motion + Lenis?
The "Experimental Sleek" aesthetic requires 60fps animations.
- **GSAP** is the industry standard for complex motion sequences and integrates perfectly with scroll triggers.
- **Framer Motion** excels at simple, reactive UI animations (like the Bento cell hover effects).
- **Lenis Scroll** provides the smooth, momentum-based scrolling experience expected in high-end design portfolios, without sacrificing performance.

### Why Tailwind CSS?
Tailwind allows for rapid styling and keeps the CSS footprint small. Its utility-first approach is perfect for building the custom, non-standard layouts required for the Bento grid.

### Why Supabase & Prisma?
Supabase offers a complete backend-as-a-service (BaaS) that scales well and simplifies the setup of PostgreSQL, Auth, and Storage. Prisma provides a type-safe ORM that ensures the technical robustness of the application.

### Why Zustand?
Zustand is significantly lighter than Redux and easier to use than Context for global state that doesn't need to trigger widespread re-renders, such as tracking the active section or controlling the floating dock state.

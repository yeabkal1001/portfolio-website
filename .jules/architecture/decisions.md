# Architectural Decisions

This document records the key architectural decisions made by the Tech Lead.

## ARCH-001: Next.js 14 App Router
- **Status**: Accepted
- **Context**: The portfolio requires high performance, SEO, and modern UX.
- **Decision**: Use Next.js 14 with the App Router.
- **Rationale**: Server Components allow for minimal client-side JS, and the App Router provides a more intuitive way to manage nested layouts and data fetching.

## ARCH-002: Supabase for Backend-as-a-Service
- **Status**: Accepted
- **Context**: Need a database, authentication, and image storage without high maintenance.
- **Decision**: Use Supabase.
- **Rationale**: It provides a managed PostgreSQL instance, a built-in auth system, and an easy-to-use storage API, which accelerates development.

## ARCH-003: GSAP and Lenis for Motion
- **Status**: Accepted
- **Context**: The "Experimental Sleek" aesthetic demands high-fidelity, smooth animations.
- **Decision**: Use GSAP for complex timelines and Lenis for smooth scroll.
- **Rationale**: GSAP is the gold standard for performance-critical web animations. Lenis provides the momentum scrolling effect that enhances the premium feel of the Bento grid.

## ARCH-004: Prisma ORM
- **Status**: Accepted
- **Context**: Ensure type safety between the database and the frontend.
- **Decision**: Use Prisma.
- **Rationale**: Prisma's auto-generated client provides excellent developer experience and catches potential schema errors at compile time.

## ARCH-005: Zustand for State Management
- **Status**: Accepted
- **Context**: Manage UI states like navigation toggle and scroll progress across components.
- **Decision**: Use Zustand.
- **Rationale**: It's more lightweight than Redux and avoids the boilerplate and potential performance pitfalls of React Context for this scale.

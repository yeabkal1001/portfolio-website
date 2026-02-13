# Database Schema

The database will use PostgreSQL managed by Supabase, with Prisma as the ORM.

## Prisma Schema

```prisma
// This is your Prisma schema file,
// learn more about it in the docs: https://pris.ly/d/prisma-schema

generator client {
  provider = "prisma-client-js"
}

datasource db {
  provider = "postgresql"
  url      = env("DATABASE_URL")
}

model Project {
  id          String   @id @default(cuid())
  slug        String   @unique
  title       String
  description String
  content     String   // MDX or HTML content
  thumbnailUrl String
  videoUrl    String?
  techStack   String[] // Array of technologies used
  liveUrl     String?
  githubUrl   String?
  featured    Boolean  @default(false)
  order       Int      @default(0)
  createdAt   DateTime @default(now())
  updatedAt   DateTime @updatedAt
  category    Category @relation(fields: [categoryId], references: [id])
  categoryId  String
}

model Category {
  id       String    @id @default(cuid())
  name     String    @unique
  projects Project[]
}

model ContactMessage {
  id        String   @id @default(cuid())
  name      String
  email     String
  subject   String?
  message   String
  createdAt DateTime @default(now())
  read      Boolean  @default(false)
}

model SiteSettings {
  id            String  @id @default("global")
  siteTitle     String
  siteDescription String
  availableForHire Boolean @default(true)
  location      String  @default("Addis Ababa, ET")
}
```

## Relationships
- **Project ↔ Category**: Many-to-One. Each project belongs to one category (e.g., "Web App", "UI/UX", "Experimental").
- **ContactMessage**: Independent table for storing form submissions.
- **SiteSettings**: Singleton table for global site configuration.

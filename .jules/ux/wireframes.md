# Wireframes

## Page: Home (Bento Grid)

### Section: Hero
**Layout**: Bento Cell (Span 8/12 columns on Desktop, Full-width on Mobile)
**Elements**:
- Headline (H1): Wide Sans "Yeabsira Kayel"
- Subheadline: "Bridging design concepts and engineering reality."
- CTA Button: "View Projects" (Primary action)
- Supporting visual: Subtle 3D background animation.

**Mobile**: Full width, centered text, prominent CTA.

---

### Section: Availability / Status
**Layout**: Bento Cell (Span 4/12 columns on Desktop)
**Elements**:
- Status Indicator: Neon green pulse dot.
- Text: "Available for Freelance".
- Location: "Addis Ababa, ET".

**Mobile**: Small bar or card above/below Hero.

---

### Section: Projects Grid
**Layout**: 12-column Bento Grid (Desktop), 1-column stack (Mobile)
**Elements**:
- **Project Card (Digital Addis)**: Large (Span 8/12).
  - Background: Video loop of the agency site.
  - Hover: Title overlay + Tech stack metadata.
- **Project Card (USP Holding)**: Medium (Span 4/12).
  - Background: Static image with glassmorphism overlay.
- **Project Card (Skin Club)**: Medium (Span 6/12).
- **Project Card (Meta)**: Small (Span 2/12).

---

### Section: Tech Stack
**Layout**: Full-width Bento Cell (Span 12/12)
**Elements**:
- Section heading (H2): "The Stack"
- Tech Marquee: Infinite horizontal scroll of:
  - React, Next.js, TypeScript, GSAP, Tailwind CSS, Three.js.
- Tech Details: Metadata in Mono font.

**Mobile**: Single row marquee, touch-draggable.

---

### Section: About & Avatar
**Layout**: Split Bento Cells (Span 6/12 + 6/12)
**Elements**:
- **Avatar Cell**: Pixel art portrait with glitch animation on hover.
- **Bio Cell**: Short professional summary in Inter (Body) + Wide Sans (Subheadings).

---

## Component Patterns

### Buttons
- **Primary**: Deep black background (#050505), neon green text (#ccff00), border 1px solid neon green.
- **Secondary**: Ghost button with neon green border.

### Bento Cells
- **Border**: 1px solid #1a1a1a (subtle).
- **Background**: #0a0a0a (slightly lighter than page bg).
- **Hover**: 2px border #ccff00 + subtle scale (1.02).
- **Padding**: 24px (Desktop), 16px (Mobile).

### Typography
- **Headings**: Syne (Wide Sans), high-contrast.
- **Body**: Inter, legible grey-white.
- **Metadata**: JetBrains Mono, neon green or grey.

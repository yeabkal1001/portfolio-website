# Design Decisions

## 1. Aesthetic Selection: "Experimental Sleek"
- **Decision**: Chose a fusion of brutalist digital elements and high-performance motion.
- **Rationale**: To differentiate from standard minimalist developer portfolios and specifically appeal to Creative Directors (Persona 2) who value "design-led engineering."

## 2. Color Palette: #050505 and #ccff00
- **Decision**: Primary background set to #050505 (not pure black) with #ccff00 (neon green) as the primary accent.
- **Rationale**: #050505 provides a deeper, more premium feel than #000000 while maintaining extreme contrast. #ccff00 is a high-vibrancy "digital" color that references the neon lights and energetic tech scene in Addis Ababa.
- **Accessibility**: All primary pairings (text on background, neon on background) exceed WCAG 2.1 AA contrast requirements.

## 3. Typography Clash: Wide Sans + Monospace
- **Decision**: Used "Syne" (Wide Sans) for headings and "JetBrains Mono" for technical metadata.
- **Rationale**: Directly implements the "Differentiation" requirement in the product vision. The Wide Sans provides creative flair, while the Monospace communicates engineering precision.

## 4. Layout: Interactive Bento Grid
- **Decision**: Adopted a rigid 12-column Bento grid that collapses to 4 columns on mobile.
- **Rationale**: Bento grids are currently the gold standard for showcasing diverse "proof of work" content (Persona 1) in a high-density, interactive format.

## 5. Animation Strategy: GSAP + Lenis Scroll
- **Decision**: Integrated Lenis Scroll for smooth momentum and GSAP for micro-interactions.
- **Rationale**: To meet the "60fps" and "Awwwards quality" success metrics. Smooth scrolling is essential for the premium, high-end feel required to impress Persona 2 and 3.

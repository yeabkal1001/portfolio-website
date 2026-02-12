Role & Goal:
You are an Awwwards-winning Creative Technologist and Senior Frontend Engineer. Build a high-performance personal portfolio for Yeabsira Kayel, a Frontend Developer & UI/UX Designer based in Addis Ababa, Ethiopia.

The goal is to build a site that bridges the gap between design concepts and engineering reality. The vibe is "Experimental Sleek"—combining clean, modern UI with raw, artistic code.

Design System & Visuals:

Theme: Deep Dark Mode. Background should be a rich, matte black (#050505) or deep charcoal (#0a0a0a), not just plain black.

Accent: Neon Green (approx #ccff00 or #39ff14). Use this sparingly for buttons, cursors, and active states to create maximum contrast.

Typography: A clash of styles. Use a massive, wide sans-serif (like 'Inter Tight' or 'Manrope') for headlines, and a technical monospace font (like 'JetBrains Mono') for metadata, location, and tags.

Avatar: Integrate a Pixel Art Avatar of Yeabsira in the Hero section. Give it a subtle "glitch" or "scanline" shader effect on hover to mix the retro pixel style with the modern sleek vibe.

Layout & Architecture (The Bento Grid):
Instead of a standard list, use a dynamic, responsive Bento Grid layout.

Hero Cell: Large text: "Yeabsira Kayel. Frontend Developer & UI/UX Designer." Subtext: "Turning design concepts into interactive realities."

Location/Status Cell: A map snippet of Addis Ababa with a live time clock. Next to it, a pulsing green indicator light with the text "Available for Freelance."

Tech Stack Cell: An infinite scrolling marquee showcasing: React, Next.js, TypeScript, Figma, Framer, GSAP, Blender, Spline.

Project Showcase (Interactive Cards):
Create specific grid cells for these projects. On hover, the cards should scale slightly and play a video loop or show a WebGL distortion effect.

Digital Addis: Label as "Tech Agency."

USP Holding: Label as "Corporate/Enterprise."

Skin Club: Label as "eCommerce/Beauty."

Portfolio: A meta-link to this current site logic.

Motion & Interaction (The X-Factor):

Stack: Next.js (App Router), Tailwind CSS, Framer Motion (for layout transitions), and GSAP (for timeline animations).

Scroll: Implement Lenis Scroll for momentum-based, buttery smooth scrolling.

3D Integration: Since I use Blender/Spline, include a subtle 3D element (like a floating geometric primitive or wireframe spline) in the background that rotates based on scroll position.

Navigation: A floating "Dock" at the bottom center of the screen (macOS style) with glass-morphism blur.

Cursor: A custom ring cursor that snaps to interactive elements and turns Neon Green on hover.

Technical Constraints:

Ensure the layout is mobile-responsive (stack the bento grid on mobile).

Use semantic HTML5.

Code must be component-based and clean.
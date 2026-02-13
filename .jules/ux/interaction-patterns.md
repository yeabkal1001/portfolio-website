# Interaction Patterns

## Scroll Behaviors
- **Smooth Scroll (Lenis)**: Implement Lenis Scroll to provide a momentum-based, high-end feel.
- **GSAP ScrollTrigger**:
  - Reveal Bento cells as they enter the viewport.
  - Subtle parallax on the 3D background primitives.
  - Floating dock navigation that minimizes or changes opacity on scroll.

## Hover States
- **Bento Cells**:
  - Scale up by 2%.
  - Border color changes from #1a1a1a to #ccff00 (Neon Green).
  - Soft neon glow effect.
- **Pixel Art Avatar**:
  - Random "glitch" distortion using CSS filters or canvas-based pixel displacement.
- **Buttons**:
  - Invert colors or add a sweeping shine effect.

## Click/Tap Behaviors
- **Project Expansion**: Clicking a project cell opens a full-screen or modal detailed view with smooth GSAP flip-style transitions.
- **Floating Dock**: Tap to jump to sections with smooth-scroll offset.
- **Mobile Gestures**: Ensure all hover effects have touch-start equivalents or are adapted for mobile taps.

## Loading States
- **Initial Load**: A custom SVG/CSS loader using the "Yeabsira Kayel" logo or a "digital construction" animation.
- **Page Transitions**: Seamless transitions between the grid and detailed views to maintain the app-like feel.
- **Image/Video Lazy Loading**: Use skeleton placeholders in the Bento grid before media assets load.

## Micro-interactions
- **Tech Marquee**: Pauses or slows down on hover to allow reading.
- **Contact Feedback**: Snappy success/error messages with monospace typography and "Experimental Sleek" styling.
- **Cursor**: Optional custom "ring" cursor that reacts to interactive elements.

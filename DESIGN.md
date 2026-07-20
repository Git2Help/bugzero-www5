---
version: alpha
name: NovaStudio Creative Agency
description: A premium, high-density landing page for a creative agency featuring kinetic typography, WebGL-enhanced backgrounds, and a sophisticated monochromatic aesthetic with electric indigo accents.
colors:
  background: "#fcfcfc"
  foreground: "#0a0a0a"
  primary: "#4f46e5"
  secondary: "#7c3aed"
  accent: "#a5b4fc"
  muted: "#888"
  border: "#eaeaea"
  dark-surface: "#080808"
typography:
  family: "Inter, system-ui, sans-serif"
  headings:
    weight: 500
    tracking: "-0.05em"
    lineHeight: "0.95"
  body:
    weight: 400
    lineHeight: "1.6"
spacing:
  section-py: "clamp(6rem, 10vw, 12rem)"
  container-max: "90rem"
rounded:
  default: "0.5rem"
  large: "1.5rem"
  extra-large: "2rem"
components:
  button-primary: "rounded-full bg-[#0a0a0a] text-white px-8 py-3.5 text-sm hover:shadow-xl"
  card-glass: "bg-white/60 backdrop-blur-md border-[#eaeaea] border"
  badge: "rounded-full border-[#e5e5e5] bg-white/60 px-4 py-1.5 text-xs"
---

## Overview
NovaStudio's visual identity is defined by a "Kinetic Precision" aesthetic. It balances a clean, minimalist foundation with high-performance motion cues including 3D CSS transforms, WebGL particle backgrounds, and liquid-gradient text effects. The interface uses a generous spacing rhythm and high typographic density to convey authority and modern craftsmanship.

## Colors
- **Base Foundation**: The primary canvas is #fcfcfc (off-white) and #ffffff, contrasted by a deep #0a0a0a (near-black) for text and dark-mode surfaces.
- **Brand Accents**: A core gradient of Indigo (#4f46e5), Purple (#7c3aed), and Blue (#2563eb) is used for emphasis, interactive states, and animated highlights.
- **Neutral Palette**: Borders utilize a light grey #eaeaea. Muted text uses #666 and #888 for hierarchy.

## Typography
- **Primary Font**: Inter (Google Fonts). Weights: 300, 400, 500, 600.
- **Hero Heading**: Uses a fluid `clamp(3.5rem, 8vw, 8.5rem)` with extreme tight tracking (-0.05em) and absolute zero or negative letter-spacing via custom kinetic animations.
- **Section Headings**: Scaled between 2.5rem and 4.5rem, maintaining a tracking-tighter profile.
- **Mono Elements**: Small uppercase labels use a mono-spaced feel with wide tracking (tracking-widest).

## Layout
- **Grid System**: A maximum width of 90rem (1440px) is maintained for main content blocks.
- **Navigation**: A sticky 16rem (64px) header with a heavy backdrop-blur (xl) and a subtle bottom border.
- **Responsive Strategy**: Heavy use of flex-col on mobile transitioning to grid-cols-12 on desktop.
- **Visual Density**: High density in feature areas and lower density (wide whitespace) in transition areas.

## Elevation & Depth
- **Surfaces**: Most cards are flat with subtle borders, but elevate on hover with `shadow-2xl shadow-black/5`.
- **Glassmorphism**: Applied to navigation, badges, and the cookie banner using `backdrop-blur-xl` and `bg-white/80` or `bg-[#101010]/95`.
- **3D Depth**: Hero text uses `perspective: 1200px` and `preserve-3d` to create physical rotation during entry animations.

## Shapes
- **Corner Radius**: Large rounded corners (1.5rem to 2rem) for testimonials and cards. Pill-shaped buttons (rounded-full) for all primary actions.
- **Accents**: Circular pulse indicators (h-2 w-2) and orbital rings in the "Method" section.

## Components
- **Sticky Header**: Includes a mega-menu dropdown with multi-column layouts (Grid 12) and feature thumbnails.
- **Service Cards**: Article elements with an aspect-ratio [4/3] image, greyscale-to-color hover transition, and an floating icon button that emerges from the bottom-left.
- **Testimonial Rail**: A horizontal scrolling container (snap-x snap-mandatory) featuring cards with organic rotation (rotate-2, rotate-1, -rotate-1) to simulate a physical editorial feel.
- **Accordions**: Massive typographic triggers with watermark numbering (e.g., "01", "02") in the background that shift on hover. Inner content uses dark-gradient cards.

## Page Sections
### Top Banner
Black high-contrast strip with an indigo pulsing dot. Essential for news/awards announcements.

### Hero Section
Centrally aligned with a WebGL canvas background. Features kinetic text that reveals with a 3D rotateX and blur transition. Includes a floating glass badge and a primary CTA.

### Client Ticker
Greyscale logo marquee with a linear gradient mask on edges to create a fading entry/exit effect. Transitions to full color on group hover.

### Agency Reel
A 16:8.2 aspect ratio video container with a dark-glass cookie banner overlay and high-contrast control buttons (Pause, Full-screen) in the top-right.

### Testimonials
An editorial layout with an asymmetrical grid. Features overlapping cards and custom navigation arrows at the bottom-right. Cards use grayscale portraits and heavy leading in typography.

### NovaStudio Method (Dark Section)
A high-contrast black section with an SVG data-connection schema. Uses animated energy pulses and schema nodes to visualize a process map.

## Motion & Interaction
- **Kinetic Reveal**: Hero text uses a custom CSS animation `kineticReveal` with translateZ and rotateX.
- **Liquid Text**: A 4-second linear infinite background-position animation for gradient text.
- **Scroll Reveal**: Global utility class for 1s cubic-bezier(0.16, 1, 0.3, 1) translateY(2rem) entry.
- **Accordion Transitions**: Uses `grid-template-rows` 0fr to 1fr transition for smooth height expansion.

## Do's and Don'ts
- **Do**: Use heavy tracking-tighter on large headings.
- **Do**: Maintain the electric indigo (#4f46e5) for all interactive pulse or highlight states.
- **Don't**: Use sharp corners; always prefer the standard rounded or large-radius profile.
- **Don't**: Remove the backdrop-blur from navigation elements.

## Accessibility
- **Skip Link**: Includes a "Skip to main content" anchor visible only on focus.
- **Aria Roles**: Navigation uses `aria-label="Main navigation"`, and buttons include `aria-expanded` and `aria-label` states.
- **Color Contrast**: Selection colors set to white text on indigo background for readability.

## Assets
1. JavaScript: https://cdn.tailwindcss.com
2. JavaScript: https://code.iconify.design/iconify-icon/2.1.0/iconify-icon.min.js
3. JavaScript: https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js
4. Analytics: https://www.googletagmanager.com/gtag/js?id=G-2M6V79H761
5. Thumbnail: https://hoirqrkdgbmvpwutwuwj.supabase.co/storage/v1/object/public/assets/assets/3f7dbc5c-f27b-4ee7-bb49-ce924886459c_320w.webp
6. Logo ABM: https://dhygzobemt712.cloudfront.net/Web/logos/dark/abm.svg
7. Logo Discord: https://dhygzobemt712.cloudfront.net/Web/logos/dark/discord.svg
8. Logo DocuSign: https://dhygzobemt712.cloudfront.net/Web/logos/dark/docusign.svg
9. Logo IDEO: https://dhygzobemt712.cloudfront.net/Web/logos/dark/ideo.svg
10. Logo Lattice: https://dhygzobemt712.cloudfront.net/Web/logos/dark/lattice.svg
11. Logo NYT: https://dhygzobemt712.cloudfront.net/Web/logos/dark/the-new-york-times.svg
12. Logo Upwork: https://dhygzobemt712.cloudfront.net/Web/logos/dark/upwork.svg
13. Video Poster: https://cdn.prod.website-files.com/686294e263eb7e215bd232f7/68c0557aa0ca3aef28f7396d_home-hero-vid-poster.webp
14. Hero Video: https://dhygzobemt712.cloudfront.net/Web/home/09-2025/home-hero.mp4
15. Card Image 1: https://hoirqrkdgbmvpwutwuwj.supabase.co/storage/v1/object/public/assets/assets/variants/e44ec1fe-2eb5-4aee-917b-f31f10e9f350/1600w.jpg
16. Card Image 2: https://hoirqrkdgbmvpwutwuwj.supabase.co/storage/v1/object/public/assets/assets/variants/e414d578-afd1-4518-9e6f-71869b5d327a/1600w.jpg
17. Card Image 3: https://hoirqrkdgbmvpwutwuwj.supabase.co/storage/v1/object/public/assets/assets/f8f2e308-3a78-44ba-ad9b-3f23f5863b94_1600w.webp
18. Testimonial 1: https://hoirqrkdgbmvpwutwuwj.supabase.co/storage/v1/object/public/assets/assets/0413dc82-d7c0-447d-aaa9-87ce398bca83_320w.webp
19. Testimonial 2: https://hoirqrkdgbmvpwutwuwj.supabase.co/storage/v1/object/public/assets/assets/b202409f-816e-4451-8ac9-bd0b04439d1b_320w.webp
20. Testimonial 3: https://hoirqrkdgbmvpwutwuwj.supabase.co/storage/v1/object/public/assets/assets/2d58e13a-35ac-4c87-af00-53519df6a64b_320w.webp
21. Avatar 1: https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?w=320&h=320&fit=crop&crop=faces&q=80
22. Avatar 2: https://images.unsplash.com/photo-1494790108377-be9c29b29330?w=320&h=320&fit=crop&crop=faces&q=80
23. Avatar 3: https://images.unsplash.com/photo-1500648767791-00dcc994a43e?w=320&h=320&fit=crop&crop=faces&q=80
24. Font: https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&display=swap

### Exported Codebase Asset Inventory
1. other: https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?w=320&amp;h=320&amp;fit=crop&amp;crop=faces&amp;q=80
   Context: index.html: markup attribute; index.html: absolute url literal
2. other: https://images.unsplash.com/photo-1494790108377-be9c29b29330?w=320&amp;h=320&amp;fit=crop&amp;crop=faces&amp;q=80
   Context: index.html: markup attribute; index.html: absolute url literal
3. other: https://images.unsplash.com/photo-1500648767791-00dcc994a43e?w=320&amp;h=320&amp;fit=crop&amp;crop=faces&amp;q=80
   Context: index.html: markup attribute; index.html: absolute url literal
4. other: http://www.w3.org/2000/svg
   Context: index.html: absolute url literal

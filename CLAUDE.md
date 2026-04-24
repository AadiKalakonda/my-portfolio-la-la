# Claude Code Instructions — my-portfolio-la-la

## Project
Personal portfolio for Adarsh Kalakonda. MS Data Science at SUNY Albany, graduating May 2026. See BRIEF.md for full context.

## Tech stack (locked)
- Next.js 15 (App Router, TypeScript)
- Tailwind CSS
- Framer Motion — page/section transitions, simple reveals
- GSAP + ScrollTrigger — scroll-linked parallax, pinning, timeline animation
- Lenis — smooth scroll (wire globally in root layout)
- React Three Fiber + drei — Three.js hero (animated graph network)
- Deployed on Vercel

## Hard rules
1. **Before generating any component, read BRIEF.md and look at every image in references/.** Match that visual language. If you haven't looked at references/, stop and look first.
2. **Use the design system from .superdesign/** once it exists. Tokens, type scale, spacing — pull from there, don't invent.
3. **No generic SaaS patterns.** No centered hero with two CTAs. No icon grids. No "meet the team" energy. If you find yourself reaching for a familiar template, stop and do something else.
4. **Metrics are first-class content.** When rendering project sections, the numbers (91% accuracy, 1.4M+ records, 30-35% reduction, etc.) should be typographically prominent, not buried in body text.
5. **Components under ~150 lines.** Split aggressively. Animation logic in custom hooks.
6. **Respect `prefers-reduced-motion`.** All GSAP/Framer animations must check this and degrade gracefully.
7. **Mobile: disable or simplify heavy parallax below 768px.** Three.js hero should have a lightweight fallback on mobile.
8. **TypeScript strict.** No `any`.
9. **Tailwind, not inline styles.** No CSS modules unless truly necessary.

## Folder structure
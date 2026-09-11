# SMM Panel — Landing Page

A responsive landing/login page for a Social Media Marketing (SMM) panel 
built to practice component-driven layout work, responsive design, and
lightweight, performance-conscious UI animation in React.

## Preview

The page is a single-scroll marketing site: a hero section with a working
sign-in form UI, a horizontally scrollable pricing carousel, an about
section, a tabbed services showcase, a 4-step process breakdown, and a
footer each section revealing itself as you scroll.

## Sections

- **Hero** — headline, sign-in form, floating rating/trust badges, and a
  decorative comet/rocket motif
- **Pricing** — horizontally scrollable, snap-scrolling pricing cards per
  platform
- **About** — brand story with a highlight image
- **Services** — tabbed service categories with a live preview panel
- **Process** — 4-step "how it works" flow
- **Footer** — links, contact info, and social channels, styled with a
  dark "galaxy horizon" background

## Tech Stack

- [React 19](https://react.dev/)
- [Vite](https://vite.dev/)
- [Tailwind CSS v4](https://tailwindcss.com/)
- [lucide-react](https://lucide.dev/) for icons

No animation or carousel library is used scroll reveals, hover states,
and the pricing carousel are all built with plain CSS transitions/keyframes
and a small `IntersectionObserver`-based `Reveal` component, to keep the
bundle light. All animations respect `prefers-reduced-motion`.

## Getting Started

Install dependencies:

```bash
npm install
```

Run the dev server:

```bash
npm run dev
```

Build for production:

```bash
npm run build
```

Preview the production build locally:

```bash
npm run preview
```

Lint:

```bash
npm run lint
```

## Project Structure

```
src/
  assets/         static images/icons
  components/     UI components (Hero, About, Services, Process, Footer, ...)
  data/           content/config for each section (easy to edit without touching JSX)
  App.jsx         page composition
  main.jsx        app entry point
```

Content for each section (copy, links, pricing plans, service list, etc.)
lives in `src/data/`, separate from the components — so wording or pricing
can be updated without touching the JSX/markup.

## Notes

- The sign-in form in the Hero section is UI-only for now; `handleSubmit`
  is a placeholder until it's wired up to a real auth backend.
- Built and tested at common breakpoints (mobile / tablet / desktop);
  the mobile nav menu, pricing carousel, and hero layout all adapt
  responsively.

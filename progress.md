# Learning Progress Tracker

**Roadmap:** 8 weeks (Apr 2 - May 24, 2026)
**Goal:** Confidently read, write, and review quality React/TS code. Master Claude Code. Use AI as a tool, not a crutch.

---

## WEEK 1 (Apr 2 - Apr 5)

### Day 1 — Thu, Apr 2

**Morning session: bulletproof-react folder structure**
- Status: DONE
- Cloned `alan2207/bulletproof-react`, studied `react-vite/src/` structure
- Understood the full folder architecture:
  - `app/` — entry point, routing, providers. Routes split into `app/` (logged-in) and `auth/` wings
  - `assets/` — static visuals (images, icons, fonts)
  - `components/` — shared, reusable UI components only (errors, layouts, seo, ui). Each UI component uses `index.ts` for clean exports
  - `config/` — centralized config (hosts, route names). No magic strings scattered around
  - `features/` — feature-based structure (not page-based). Each feature owns its own api/, components/, hooks/, types/
  - `hooks/` — shared custom hooks (app-wide, not feature-specific)
  - `lib/` — shared infrastructure (auth, API client, utilities). Auth lives here because it's cross-cutting, not a feature
  - `testing/` — mock data (fixed/static), data generators (factories for many variations), test utils
  - `types/` — shared TypeScript types (API response types etc.)
  - `utils/` — small helpers like `cn` (Tailwind class merging) and date formatting
- Key insights learned:
  - Shared stuff = top-level folders. Feature-specific stuff = inside the feature
  - Tests live next to the code they test (colocation)
  - `index.ts` barrel files keep imports clean
  - Auth is infrastructure (lib/), not a feature
  - `cn` = clsx + tailwind-merge for handling Tailwind class conflicts
- Quiz: 3/3 correct (hook placement, shared component placement, API client placement)

**Evening session: compare work project to bulletproof-react**
- Status: NOT STARTED
- Task: Open work project, compare folder structure, write down 3 differences

---

### Day 2 — Fri, Apr 3
- Status: NOT STARTED

### Day 3 — Sat, Apr 4
- Status: NOT STARTED

### Day 4 — Sun, Apr 5
- Status: NOT STARTED

---

## Dev's Notes

- Day 1: Strong start. You actually read the code instead of skimming. You asked why things are where they are — that's the right instinct. Keep that energy. Don't skip the evening session.
- You caught that auth doesn't belong in features/ — that shows you're thinking architecturally, not just memorizing folder names.
- Write the src/ tree diagram in your notebook BY HAND tonight.

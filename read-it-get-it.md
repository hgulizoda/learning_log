# Read It, Get It

Learning to read production codebases and understand why good code is structured the way it is.

---

## Apr 2, 2026

**Studied:** `alan2207/bulletproof-react` — project architecture (`react-vite/src/`)

- Learned feature-based folder structure: `features/`, `components/`, `lib/`, `hooks/`, `types/`, `utils/`
- Key insight: shared code lives at top level, feature-specific code stays inside its feature folder
- Auth is infrastructure (`lib/`), not a feature — it cuts across the whole app
- Tests go next to the code they test (colocation), not in a separate global folder
- Barrel exports (`index.ts`) keep imports clean
- `cn` utility = `clsx` + `tailwind-merge` for handling Tailwind class conflicts
- Mock data = fixed/static test objects. Data generators = factories that produce many variations
- Route structure mirrors app sections: `routes/app/` for logged-in, `routes/auth/` for auth pages

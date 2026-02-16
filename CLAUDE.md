# rpedroni-labs-pages

Public GitHub Pages repo for hosting static pages from the rpedroni-labs MVP factory.
Created to serve content that needs to be publicly accessible (no auth, no build step).

- **Repo**: `rpedroni/rpedroni-labs-pages` (PUBLIC)
- **GitHub Pages**: legacy deploy from `main` branch
- **Custom domain**: `rpedroni.com.br/rpedroni-labs-pages/`
- **Related**: `rpedroni/rpedroni-labs` (private monorepo)

## Architecture

Single self-contained HTML files. No frameworks, no build step, no dependencies.
Each file is a standalone page with inline CSS + JS. Google Fonts loaded via CDN.

```
rpedroni-labs-pages/
├── CLAUDE.md          # This file
└── treino/
    └── ricardo/
        ├── index.html  # Workout tracker page
        └── avatar.png  # Ricardo's profile photo
```

## Workout Tracker (`/treino/ricardo/`)

### What it is
A mobile-first personal trainer workout page for Ricardo, following the **MaxResults methodology** by trainer **Luisão Ribeiro**. Functions like a premium native fitness app (dark theme, 480px max-width).

### Live URL
`https://rpedroni.com.br/rpedroni-labs-pages/treino/ricardo/`

### Design
- **Aesthetic**: Dark luxury athletic — deep layered blacks, warm/cool accent colors
- **Fonts**: Outfit (display/headers) + DM Sans (body) via Google Fonts
- **Colors**:
  - Warmup blocks: pink (`#fb7185`)
  - Mobility blocks: purple (`#a78bfa`)
  - MaxLift blocks: amber (`#f59e0b`)
  - Cardio blocks: cyan (`#22d3ee`)
  - Completed: green (`#34d399`)
- **Effects**: Noise grain overlay, ambient top glow, gradient brand text, gradient-border avatar with glow, staggered card reveals on initial load, spring-physics checkbox animations, CSS grid detail expand/collapse

### Workout Structure (4 blocks per training day)
1. **Aquecimento** (warmup) — general activation, ~5-8 min
2. **Mobilidade** — chain-specific mobility, ~5-8 min
3. **MaxLift** — strength training, 25-30 min
4. **Cardio** (MaxFight or MaxStep), 25-30 min

Warmup and mobility exercises vary by the day's focus:
- **Cadeia Posterior** (Mon/Thu): cat-cow, 90/90 hip, hamstring stretch
- **Cadeia Anterior** (Tue/Fri): thoracic rotation, hip flexor, pass-through

### Week layout (Feb 16-20, 2026)
| Day | Focus | Cardio |
|-----|-------|--------|
| Seg 16 | Treino 1 — Cadeia Posterior (Mix 1) | MaxFight |
| Ter 17 | Treino 2 — Cadeia Anterior (Mix 1) | MaxStep |
| Qua 18 | Descanso | — |
| Qui 19 | Treino 1 — Cadeia Posterior (Mix 2) | MaxFight |
| Sex 20 | Treino 2 — Cadeia Anterior (Mix 2) | MaxStep |

### Features
- **Sticky header**: Avatar, athlete name, day label, progress bar
- **Weekly goals card**: "Meta da Semana" with strength/cardio/assessment goals (data in `WEEKLY_GOALS` array)
- **Day switcher**: Mon-Fri buttons, rest day disabled, green dot on completed days
- **Exercise cards**: Checkbox to complete, expand for equipment + tips
- **Progress tracking**: Per-block counters, overall % bar, localStorage persistence
- **Session complete banner**: Appears at 100% with scale-up animation
- **Week overview**: Expandable full-week summary

### Key technical decisions
- **No full re-render on exercise toggle**: `toggleExercise()` updates DOM in-place (toggles `.completed` class, updates block counters + progress bar). This preserves expanded detail panels on other exercises.
- **Detail expand animation**: Uses `grid-template-rows: 0fr → 1fr` instead of `max-height` hack for smooth content-aware transitions.
- **Initial load animations**: Scoped to `.initial-load` class on the `<main>` element, removed after 600ms to prevent re-triggering on state changes.
- **Storage key versioned**: `maxresults-ricardo-2026-02-16-v2` — bump the version when block structure changes to avoid stale progress data.

### How to update for a new week
1. Update `WEEK` array with new dates, exercises, and mix numbers
2. Update `WEEKLY_GOALS` array with new goals
3. Bump `STORAGE_KEY` version (e.g., `-v3`)
4. Update `header-date` text in `renderWorkout()` and footer date
5. Warmup/mobility blocks are shared constants (`WARMUP_POSTERIOR`, `WARMUP_ANTERIOR`, `MOBILITY_POSTERIOR`, `MOBILITY_ANTERIOR`) — update if the trainer changes the routine

### Deploying
```bash
cd /Users/rpedroni/Desktop/rpedroni/rpedroni-labs-pages
git add . && git commit -m "message" && git push origin main
# GitHub Pages (legacy) auto-deploys from main, takes ~30s
# Check: gh api repos/rpedroni/rpedroni-labs-pages/pages/builds/latest -q '.status'
```

## UI strings
All hardcoded UI text is in **Portuguese (pt-BR)**. Watch for diacritics: Sessão, Concluída, Luisão, etc.

## Future ideas (not started)
- Generate weekly workout pages from the personal-trainer-bot AI in rpedroni-labs
- Add more athletes (different `/treino/{name}/` paths)
- PWA manifest + service worker for offline use
- Weekly history / streak tracking

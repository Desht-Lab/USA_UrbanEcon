# Design System — Kazakhstan Regional Observatory (frontend)

A reference summary of the frontend design code. The design lives in three CSS files
(`frontend/src/index.css`, `frontend/src/App.css`) plus inline styles in `App.jsx`.
It is a **CSS-custom-property-driven, dark-first theme** with a light variant. No CSS
framework (no Tailwind/MUI) — hand-written, class-based CSS.

---

## Typography

Two font stacks are loaded at different layers:

- `index.css` imports **Space Grotesk** (Google Fonts) and sets it as the root family.
- `App.css` imports **Gotham** (from a Desht-Lab GitHub stylesheet) and overrides
  `.page` / `body` / form elements to use `"Gotham", "Inter", "Segoe UI", system-ui, sans-serif`.

Net effect: **Gotham wins for app content**; Space Grotesk only applies outside `.page`.
This is a likely inconsistency to clean up.

Base: `line-height: 1.5`, `font-weight: 400`, `color-scheme: dark`.

---

## Theming

Tokens defined on `:root` (dark) with a `[data-theme="light"]` override.

| Token | Dark | Light |
|---|---|---|
| `--bg` | `#0f1115` | `#f8fafc` |
| `--fg` | `#e5e7eb` | `#0f172a` |
| `--muted` | `#9ca3af` | `#475569` |
| `--panel` | `#14171d` | `#eeedeb` |
| `--card` | `#16191f` | `#ffffff` |
| `--accent` | `#376c8a` (teal) | `#e5b983` (gold) |
| `--accent-2` | `#4f86a4` (teal) | `#e4c7a1` (gold) |
| `--nav-accent` | `#e5b983` (gold) | `#376c8a` (teal) |
| `--nav-accent-2` | `#f0cb9b` | `#4f86a4` |
| `--border` | `#222733` | `#e9e1d7` |
| `--accent-shadow` | `rgba(55,108,138,.35)` | `rgba(229,185,131,.35)` |

**Notable:** `--accent` and `--nav-accent` swap roles between themes (teal ↔ gold).

### Map label tokens
Floating map labels and maplibre popups have dedicated tokens (`--label-bg`, `--label-fg`,
`--label-border`, `--label-shadow`). They deliberately stay **light-on-dark in dark mode**
and **invert in light mode**, so labels remain legible against the basemap regardless of UI theme.

- Dark: `--label-bg: rgba(255,255,255,.95)`, `--label-fg: #0b1120`
- Light: `--label-bg: rgba(15,23,42,.92)`, `--label-fg: #f8fafc`

---

## Visual language

- **Rounded floating cards**: `border-radius: 12–20px`, 1px borders (`var(--border)`),
  layered shadows (`0 10–12px 30px rgba(0,0,0,.14–.18)`).
- **Gradient page background**: two radial gradients layered over `--bg`.
- **Pill / gradient accents** for active states — `.pill-button.active` uses an accent
  gradient with a glow shadow (`box-shadow: 0 8px 24px var(--accent-shadow)`).
- **Sticky topbar** with `backdrop-filter: blur(10px)` + `color-mix` translucency.
- **Hover dropdowns** (`.complexity-dropdown`) animated via opacity/transform/visibility transitions (~0.16s ease).
- Transitions generally `0.15–0.2s ease`.

---

## Layout

- **CSS Grid** throughout.
  - Main `.layout`: `grid-template-columns: 2fr 1fr` (map spans both columns).
  - Region page uses **named grid areas**: `map`, `text`, `climate`, `eth`, `pyramid`,
    `industry1`–`industry3`.
- Spacing rhythm: page padding `24px`, gaps `12–16px`, `clamp()` for fluid padding
  (`clamp(16px, 4vw, 32px)`).
- Map shells use fluid/viewport heights: `clamp(420px, 60vh, 720px)`, `60vh`, etc.

### Responsive breakpoints
`1100px` · `1080px` · `900px` · `720px` · `480px` — progressively collapse multi-column
grids to single column, shrink map heights, and stack the topbar.

---

## Component families

Distinct styled blocks per data-viz section:

- **Stat cards** — `.stat-grid` (auto-fit `minmax(180px,1fr)`), uppercase labels, 22px values.
- **Economic complexity board** — `.complexity-board` with absolutely-positioned columns/rows
  and an SVG ribbon layer (`.complexity-ribbon`, `stroke-width: 8`, `opacity: .34`) connecting items.
- **Population pyramid** — male bars `#8abafc` (blue), female bars `#f9a8c4` (pink);
  `.pyramid-row` grid `1fr 80px 1fr`; fixed tooltip.
- **Ethnicity** — bars + auto-fit legend with swatches; reuses male/female blue/pink.
- **Climate** — bars + legend grid (`.climate-legend-item` grid `16px 48px 1fr 60px`).
- **Industry** — horizontal bars (`.industry-row` grid `1fr 3fr 140px`), accent-filled.
- **Trade** — treemap grid (auto-fit `minmax(260px,1fr)`), flow-switch buttons, legend pills.
- **SDG** — pill-shaped chips with round swatches.

Charts use **d3plus**, with theme-override hacks, e.g.
`.d3plus-Legend text { fill: var(--fg) !important }` and light-theme axis overrides.

---

## Known cleanup candidates

- **Dual-font setup** (Space Grotesk vs Gotham) — pick one.
- **Remote `@import`** from a raw GitHub URL (`App.css:1`) — render-blocking external dependency.
- **Undefined tokens referenced**: `--surface` (line ~823), `--text-muted` (trade legends),
  `--bg-grad-1/2` (only defined in the light theme, fall back to hardcoded values in dark).
- **Duplicated `.climate-card` rule** (defined twice).

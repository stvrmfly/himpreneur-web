# DESIGN.md — HIMPRENEUR visual system

Authoritative visual reference. On visual decisions this wins; on strategy/voice, PRODUCT.md wins.

## Color (default theme; tokens in `:root`)
- `--primary` **#0A1628** — deep navy. Dark sections: hero, pillars, contact, footer.
- `--surface` **#FFFFFF**, `--surface-warm` **#F2F5F9** (neutral off-white, faint navy tint — NOT warm cream), `--surface-mid` **#E7ECF3**. Light sections + cards.
- `--accent` **#C9A96E** — gold. Decorative use (dividers, borders, bars) and gold text ON DARK only.
- `--accent-ink` **#7a5c2e** — deep gold, used for gold TEXT on light backgrounds (contrast-safe ≥4.5:1). Eyebrows/tags/labels/roles on light use this.
- `--text-primary` **#0A1628**, `--text-secondary` **#3d4f6b**, `--text-muted` **#52617a** (darkened for AA on light).
- Alt themes: `data-theme="maroon"` (oxblood #6B0D17 primary), `data-theme="white"` (navy #1B2A4A on true off-white). Gold accent constant across all.
- **Strategy:** Committed dark navy carries the hero/pillars/contact; light sections are near-neutral off-white; gold is the single accent. Do not introduce new hues in variants.

## Type
- **Display: Bricolage Grotesque** (opsz 12–96, weights 400–800). All headings, hero wordmark, names, titles. Bold, contemporary, slight character.
- **Body: Hanken Grotesk** (300–700, incl. italic). All body copy, labels, meta, buttons.
- Pairing logic: one grotesque display + one clean grotesque body (contrast by weight/scale, not by family switch). Do NOT reintroduce serif display or a third family.
- Hero wordmark is large, tracked tight; eyebrows/labels are small uppercase tracked (Hanken).

## Layout & surface
- Fixed top nav (navy, blurred), single long scroll, full-viewport hero.
- Corners: cards/photos `border-radius` 12–20px (never 32px+). Photo frames 14px, portrait 5:6.
- Shadows: soft warm shadow scale (`--shadow-sm/md/lg`); avoid pairing a 1px border with a big blur on the same element.
- Section rhythm: heading → gold divider → subtitle → content. (No repeated eyebrow label above every section — removed.)
- Batik *kawung* dot motif as low-opacity section background texture (cultural, keep).

## Components
Nav · Hero (wordmark + typewriter tagline + 3 animated stat counters) · Org chart (tree: Ketua → Sek/Bendahara → 6 divisi Koor/Wakoor, portrait photo frames) · Staff carousel (stacked-deck cards, koordinator default front, prev/next arrows + dots) · Pillars (4 mascot cards, dark) · Vision/Mission · Program slider (photo cards → detail modal with 2 photos) · Gallery · Contact (dark) · Floating theme switcher.

## Motion
- Loader: logo pulse → white flash reveal (~0.8s).
- Scroll reveals: fade/slide-up via IntersectionObserver `.visible` class (staggered).
- Hero: typewriter tagline; stat counters animate on view.
- Carousel: stacked-deck slide transition (cubic-bezier ease-out).
- All motion respects `prefers-reduced-motion: reduce`. Ease-out curves, no bounce.

## Accessibility (non-negotiable)
- Body text ≥4.5:1. Gold text on light uses `--accent-ink`.
- Interactive elements keyboard-operable; program cards are `role=button tabindex=0` with Enter/Space.
- Global `:focus-visible` gold outline. Touch targets padded to ≥24px via `::after`.

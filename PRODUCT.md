# PRODUCT.md — HIMPRENEUR BINUS @Bandung

**Register:** brand (design IS the product — a single-page landing site for a student organization).

## What it is
Public landing page for **HIMPRENEUR**, the student entrepreneur association of BINUS University, Bandung region. Single static page (`index.html`, HTML/CSS/JS, no framework) served locally via XAMPP. Sections: hero, profile/history, struktur organisasi (org chart + staff carousel), pillars, vision/mission, program kerja (activity slider + detail modals), gallery, contact.

## Audience
Prospective and current BINUS Bandung students, faculty, and partner brands. Indonesian-language. They come to gauge the org's credibility, see who runs it, and browse its programs/activities.

## Brand personality (three words)
**Confident · warm · contemporary-Indonesian.** Energetic student-entrepreneur spirit — the tagline is "Kreatif, Solid, Berdampak" (Creative, Solid, Impactful) and "To the Move and Beyond". Credible but not corporate-stiff; youthful but not childish.

## Voice
Warm, motivational, first-person-plural ("kami"). Indonesian. Celebrates people and impact. Not jargon-heavy, not ironic.

## Identity anchors (do not lose these)
- **Navy + gold** as the core brand colors (BINUS heritage + achievement/gold).
- **Cultural identity**: batik *kawung* dot motif in section backgrounds; the lightbulb-hot-air-balloon **mascot** logo. These differentiate it from generic student-org / startup templates — keep them.
- Real member **photography** (ID-card style portraits) drives the org chart and staff carousel.

## Anti-references (what it must NOT become)
- Not a generic SaaS/startup landing (gradient-hero, big-metric template, sterile).
- Not corporate/institutional-stiff.
- Not "AI-template": avoid cream/parchment warm-neutral defaults, avoid an eyebrow label above every section, avoid reflex serif pairings (Playfair/Crimson). (These were already removed in an accessibility+distinctiveness pass.)

## Constraints
- Single file, vanilla HTML/CSS/JS, no build step. Served by XAMPP at `localhost/HIMPRENEUR/`.
- Must stay accessible: WCAG AA contrast, keyboard-operable controls, visible focus, reduced-motion support.
- Three color themes exist (default navy, maroon, blue) via `data-theme` + localStorage.

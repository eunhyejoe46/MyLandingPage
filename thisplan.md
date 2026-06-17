# Travel Archive Website Plan (Updated v2)

## 1. Project Overview

### Project Concept

A minimal and emotional travel archive website that combines personal
travel photography, magazine-style storytelling, and future merchandise.

The website is not a simple travel information blog.

It focuses on:

-   Original travel photos
-   Personal travel stories
-   Hidden local experiences
-   Curated travel inspiration
-   Photo-based goods

Core idea:

"Places become memories, memories become stories."

------------------------------------------------------------------------

# 2. Brand Direction

## Brand Identity

**Site name: zzoinn**

Apple-inspired minimal design + travel magazine experience.

Keywords:

-   Clean
-   Elegant
-   Emotional
-   Modern
-   Visual storytelling

The website should feel like opening a high-quality travel magazine —
with one warm, playful moment at the very front door (see Section 3).

------------------------------------------------------------------------

# 3. Homepage Concept

## Main Hero Experience

The homepage opens with a globe-centered entrance moment, now built as
a two-stage interaction.

### v0 concept (original)
A small rotating globe.

### v1 concept (first revision)
A large, realistic 3D globe in the center of the screen — earth
texture, natural lighting, interactive country selection.

### v2 concept (current — hand-drawn entrance)

**Stage 1 — Landing**

-   On first load, only the globe is visible: large, centered, no nav
    bar, no text yet.
-   Visual style shifts from photoreal to **hand-drawn, illustrated
    3D** — sketch-line continents, soft toy-like shading, a doodle
    globe rather than a literal earth photo.
-   The globe floats and drifts freely (gentle bob + spin, idle
    motion), giving the first screen a playful, alive feeling before
    any UI appears.

**Stage 2 — After Click**

-   Visitor clicks the globe to enter the site.
-   The globe animates into a half-globe (lower half cropped), docking
    at the top of the page like a horizon band.
-   A small, cute character walks back and forth along the curved top
    edge of that half-globe — a little continuous animation living in
    the header area.
-   The rest of the homepage (navigation, search, magazine stories)
    reveals beneath this header band.

**Open questions to settle during build:**

-   Exact click target — the whole globe, or a small "enter" hint near
    it?
-   How the character's walk path and the half-globe band resize on
    mobile.

------------------------------------------------------------------------

# 4. Homepage User Experience

## First Screen — Two-Stage Flow

Stage 1 — Landing:
Large hand-drawn globe only, centered, idle floating motion

↓ (visitor clicks the globe)

Stage 2 — Entered:
Half-globe header band, walking character

↓

Top navigation (zzoinn ←  /  → Magazine · Goods · 🌙)

↓

Travel search bar

↓

Featured travel stories

------------------------------------------------------------------------

## Search Feature

Position:

Above the globe / below the entered-state header

Text:

"오늘 어떤 여행을 하고 싶나요?"

Search examples:

-   조용한 바다가 있는 여행
-   현지 맛집을 찾는 여행
-   혼자 걷기 좋은 도시
-   사진 찍기 좋은 장소

The search is emotion-based, not only location-based.

------------------------------------------------------------------------

# 5. Navigation Structure

## Layout (Updated)

-   **Left:** site name / logo — **zzoinn**
-   **Right:** nav tabs — Magazine · Goods — with the dark mode toggle
    (☀️ / 🌙) as the rightmost element

## Main Menu

Keep minimal.

### Magazine

Travel stories and recommendations.

Includes:

-   Destination stories
-   Hidden local places
-   Food experiences
-   Travel moments

### Goods

Photo-based products.

Includes:

-   Postcards
-   Photo prints
-   Frames
-   Travel collections

------------------------------------------------------------------------

# 6. Content Strategy

## Magazine

Main content format:

Photo first → Story → Information

Article structure:

1.  Hero image

2.  Personal story

3.  Location information

4.  Local recommendations

5.  Photo gallery

------------------------------------------------------------------------

# 7. Differentiation Strategy

## Hidden Local Experiences

Focus on discovering meaningful places.

Examples:

Not:

"Popular tourist attraction"

Instead:

"A small cafe discovered while walking through a quiet street"

------------------------------------------------------------------------

## Personal Perspective

The value comes from:

-   Personal experience
-   Original photography
-   Emotional storytelling

------------------------------------------------------------------------

# 8. Design System

## Style

Minimal travel magazine.

Reference:

-   Apple website
-   Premium editorial websites

Principles:

-   Large images
-   Large typography
-   Plenty of white space
-   Smooth animations

Avoid:

-   Complex menus
-   Too many categories
-   Heavy visual effects

## Scope note — where the playful style lives

The hand-drawn, playful style (Section 3, Stage 1–2: the globe and its
walking character) is intentionally limited to the hero moment.
Everything else — navigation, typography, cards, layout — stays inside
the clean, minimal Apple-inspired direction. The hero is the one place
for warmth and personality; the rest stays quiet on purpose.

------------------------------------------------------------------------

## 8-1. Dark Mode System

### Toggle

-   Position: top navigation, rightmost element — after the
    Magazine/Goods tabs, opposite the zzoinn logo on the left
-   Icon: ☀️ (light mode) / 🌙 (dark mode), crossfade + rotate
    transition on switch
-   Default: follows the visitor's OS setting (`prefers-color-scheme`)
    on first load

### Color Tokens

| Token | Light (Day) | Dark (Night) |
|---|---|---|
| Background | `#EEEBE4` warm stone paper | `#10131A` night ink |
| Elevated surface | `#F8F6F1` | `#161A22` |
| Text (primary) | `#1A1C20` | `#ECEAE2` |
| Text (soft) | `#62646C` | `#A2A6B3` |
| Accent | `#D89A3E` sunlight amber | `#96A8E4` moonlight periwinkle |
| Hairline | `rgba(26,28,32,.10)` | `rgba(255,255,255,.10)` |

### Signature Concept

The dark mode toggle stays tied to the homepage globe, not just a flat
color swap:

-   In light mode, the globe's lit hemisphere glows sunlight amber.
-   In dark mode, the same hemisphere shifts to moonlight periwinkle.
-   Switching theme reads as "turning the world from day to night,"
    reinforcing the globe as the brand's core visual identity.

------------------------------------------------------------------------

# 9. Future Monetization

## Phase 1

Build audience:

-   Magazine content
-   Travel archive
-   Photography collection

## Phase 2

Launch Goods:

-   Postcards
-   Prints
-   Frames

## Phase 3

Expand:

-   Community
-   User travel collections
-   Collaboration products

------------------------------------------------------------------------

# 10. Development Priority

## MVP Version

Build first:

1.  Homepage
2.  Two-stage globe entrance (floating hand-drawn globe → click →
    half-globe header + walking character)
3.  Travel search UI
4.  Magazine pages
5.  Photo gallery

Later:

-   Community
-   User accounts
-   Shopping system

## Assets Needed (new)

-   Hand-drawn style 3D globe (illustrated continents, soft shading —
    model or sprite, not a literal earth photo)
-   Walking character (simple sprite sheet or CSS/SVG animation,
    matches the "cute" tone of the hero)

------------------------------------------------------------------------

# 11. Progress Log

## v1 — Homepage Draft

Built as a single static `index.html`:

-   Top navigation (Magazine / Goods) with dark mode toggle
-   Emotion-based search bar + quick-search chips
-   Minimal grid-sphere globe placeholder, with day/night color sync
-   4 magazine story cards (placeholder copy + gradient thumbnails)
-   Light/dark theme via CSS variables, no real photos yet
-   Placeholder brand name used: "MERIDIAN"

## v2 — Built

1.  Two-stage entrance implemented: a hand-drawn-style floating globe
    (SVG, sketch-line continents via an `feTurbulence` filter, idle
    bob + rotation-pulse animation) shown alone on load → click docks
    it as a half-globe header band → a small character patrols back
    and forth on top of it (Section 3).
2.  Navigation reorganized: **zzoinn** on the left, Magazine/Goods tabs
    + dark mode toggle on the right (Section 5).
3.  Brand renamed from the placeholder "MERIDIAN" to **zzoinn**
    everywhere (logo, footer, page title).

Status: built in `index.html` as a single self-contained file (inline
CSS/JS, no external assets besides Google Fonts).

## Next Steps

-   Fine-tune exact pixel sizing/position of the docking globe and
    walker by eye in the browser — current values are reasonable
    defaults, not pixel-tested against a live preview.
-   Replace the placeholder hand-drawn globe with a more refined
    illustration/asset if the current sketch-filter look isn't quite
    right.
-   Replace gradient thumbnails with real travel photography.
-   Wire the search bar to actual magazine content; build out the
    Magazine article template (Section 6) and Goods page.

------------------------------------------------------------------------

# Final Concept Statement

A minimal travel magazine platform where a rotating world leads visitors
to stories, photos, and memories from around the globe.

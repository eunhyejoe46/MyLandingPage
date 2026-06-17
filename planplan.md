# Travel Archive Website Plan (Updated)

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

Apple-inspired minimal design + travel magazine experience.

Keywords:

-   Clean
-   Elegant
-   Emotional
-   Modern
-   Visual storytelling

The website should feel like opening a high-quality travel magazine.

------------------------------------------------------------------------

# 3. Homepage Concept

## Main Hero Experience

The homepage is centered around a realistic 3D globe.

### Previous concept:

A small rotating globe

### Updated concept:

A large globe placed in the center of the screen.

Features:

-   Realistic earth texture
-   Natural lighting
-   Smooth rotation animation
-   Minimal UI around the globe
-   Interactive country selection

The globe is the main visual identity of the brand.

------------------------------------------------------------------------

# 4. Homepage User Experience

## First Screen

Layout:

Top navigation

↓

Travel search bar

↓

Large interactive globe

↓

Featured travel stories

------------------------------------------------------------------------

## Search Feature

Position:

Above the globe

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

------------------------------------------------------------------------

## 8-1. Dark Mode System (Added)

### Toggle

-   Position: top navigation, far right
-   Icon: ☀️ (light mode) / 🌙 (dark mode), crossfade + rotate transition on switch
-   Default: follows the visitor's OS setting (`prefers-color-scheme`) on first load

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

The dark mode toggle is tied directly to the homepage globe, not just a
flat color swap:

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
2.  Realistic interactive globe
3.  Travel search UI
4.  Magazine pages
5.  Photo gallery

Later:

-   Community
-   User accounts
-   Shopping system

------------------------------------------------------------------------

# 11. Progress Log

## v1 — Homepage Draft (current)

Built as a single static `index.html`:

-   Top navigation (Magazine / Goods) with dark mode toggle
-   Emotion-based search bar + quick-search chips
-   Minimal grid-sphere globe placeholder, with day/night color sync
-   4 magazine story cards (placeholder copy + gradient thumbnails)
-   Light/dark theme via CSS variables, no real photos yet

## Next Steps

-   Replace gradient thumbnails with real travel photography
-   Build the real interactive 3D globe (e.g. Three.js + earth texture,
    country selection) to replace the placeholder sphere
-   Wire the search bar to actual magazine content
-   Build out Magazine article template (section 6) and Goods page

------------------------------------------------------------------------

# Final Concept Statement

A minimal travel magazine platform where a rotating world leads visitors
to stories, photos, and memories from around the globe.

# Exploration Servers – Homepage Wireframe Specification (Detailed)

## 1. Document Purpose

This document defines the **structural wireframe** for the Exploration Servers homepage.

It is intended to bridge strategy and implementation by specifying:

- information hierarchy
- desktop and mobile layout
- section stacking and spacing
- surface treatment (dark / parchment / mixed)
- grid behavior
- navigation behavior
- sticky / scroll patterns
- component priorities
- CTA placement

This is **not** a visual design comp.  
It is a structural and behavioural specification for building the homepage in Tailwind.

---

## 2. Core Page Intent

The homepage must communicate, in order:

1. This is a distinct Minecraft experience
2. Exploration is the core progression loop
3. The world is structured and meaningful
4. There are servers available to join

### Strategic Rule
The page should feel like a **concept landing page with playable destinations attached**, not a generic server homepage and not a feature dump.

---

## 3. Global Layout Rules

## 3.1 Page Widths

Use three layout widths:

- **max content width:** 1200px
- **reading width:** 760px
- **narrow emphasis width:** 640px

### Usage
- 1200px for hero, feature grids, server cards
- 760px for explanatory copy
- 640px for “Why This Exists” and other editorial moments

---

## 3.2 Section Padding

### Desktop
- top/bottom section padding: **96px**
- hero top padding under nav: **120px minimum**
- internal card padding: **32px**

### Tablet
- top/bottom section padding: **72px**

### Mobile
- top/bottom section padding: **56px**
- internal card padding: **20–24px**

---

## 3.3 Surface Rhythm

The page should alternate surfaces to create pacing.

### Recommended section surface pattern
1. Hero → **dark**
2. The Shift → **dark**
3. What This Changes → **parchment**
4. The Experience → **dark**
5. Core Systems → **dark**
6. Exploration Servers → **parchment**
7. Why This Exists → **parchment or soft mixed**
8. Final CTA → **dark**

### Reason
This creates editorial contrast and prevents the entire page from becoming one long dark slab.

---

## 3.4 Vertical Flow

Every section should have:
- a clear entry point
- one dominant message
- one structural pattern
- one optional supporting pattern

Avoid mixed layouts inside a single section unless there is a clear reason.

---

## 4. Breakpoints

Use these working breakpoints:

- **mobile:** < 768px
- **tablet:** 768px to 1023px
- **desktop:** 1024px+
- **wide desktop:** 1280px+

---

## 5. Header / Navigation Wireframe

## 5.1 Desktop Header

### Placement
- Fixed or sticky at top
- Sits over hero
- Full-width container with centered max-width inner wrapper

### Inner structure
- Left: wordmark / logo
- Center or right: nav links
- Far right: primary CTA button

### Desktop nav items
- Home
- How It Works
- Servers
- Discord

### CTA
- Explore Servers

### Height
- 72px desktop header height

### Behaviour
- Starts transparent over hero
- On scroll, transitions to semi-opaque dark surface with subtle blur or solid dark fill
- Border or bottom separator appears once page scrolls past hero threshold

### Sticky rule
Sticky header is recommended.  
Do not make it oversized or app-like.

---

## 5.2 Mobile Header

### Structure
- Left: logo / wordmark
- Right: menu trigger
- CTA should not appear as a separate button in the top row on small mobile unless space allows

### Height
- 64px

### Mobile menu
- Full-width slide-down panel or right-side sheet
- Contains:
  - Home
  - How It Works
  - Servers
  - Discord
  - Explore Servers CTA at bottom

### Behaviour
- Menu should lock body scroll while open
- Avoid nested menus

---

## 6. Hero Section Wireframe

## 6.1 Purpose
Set the concept, emotional tone, and immediate orientation.

## 6.2 Desktop Layout

### Height
- Preferred: **min-height 90vh**
- Acceptable: **min-height 820px**
- Do not make hero too shallow

### Layout pattern
**Split-column hero**

#### Left column (primary)
- eyebrow / optional small label
- large headline
- supporting paragraph
- CTA row
- optional small trust/info strip beneath CTAs

#### Right column (secondary visual)
- atmospheric world/map visual
- could be:
  - stylised map fragment
  - terrain screenshot montage
  - abstract region overlay
  - named-world visual motif

### Width split
- 52% text / 48% visual
or
- 50 / 50 if visual treatment is strong

### Text width
- headline max width: ~10–12 words per line
- supporting paragraph width: 480–560px max

### CTA row
- Primary: Explore Servers
- Secondary: How It Works

### Optional tertiary micro-info row
Could include:
- structured discovery
- named world
- persistent progression

Keep this very light.

---

## 6.3 Mobile Hero Layout

### Height
- auto height, but should still feel dominant
- top padding generous enough to avoid cramped first impression

### Stack order
1. headline
2. subtext
3. CTA row
4. hero visual

### CTA stacking
- Primary button full-width or near-full-width
- Secondary button below it
- On larger mobile, buttons may sit side by side if readable

### Visual
- Move below text
- Reduce decorative complexity
- No oversized art pushing CTAs too far down

---

## 6.4 Hero Surface & Tone

- Dark base surface
- Optional soft texture or gradient
- Visual should not compete with headline legibility
- Preserve strong contrast

---

## 7. The Shift / Problem Framing Section

## 7.1 Purpose
Frame the gap in vanilla exploration without turning the page into a complaint page.

## 7.2 Desktop Layout

### Pattern
**Three-card horizontal contrast row** above a short closing statement

#### Row
- 3 equal-width cards
- Each card contains one short statement
- Cards should have consistent height

#### Below row
- A single stronger line:
  “Exploration exists. It just isn’t the reason you play.”

### Grid
- desktop: 3 columns
- tablet: 3 columns if space allows, else 1x3 stacked
- mobile: single-column stacked cards

### Card treatment
- dark-on-dark or dark-surface variation
- restrained border
- no icon necessary, though subtle icons are acceptable

---

## 7.3 Section Width
- row uses full content width (up to 1200px)
- closing line should use narrower reading width

---

## 8. What This Changes Section

## 8.1 Purpose
Define the concept in operational terms.

## 8.2 Desktop Layout

### Pattern
**Two-column editorial explainer**

#### Left column
- section heading
- short intro paragraph
- key line / pull quote

#### Right column
- 3 concept pillars as stacked cards or list blocks

### Split
- 45% / 55% or 50% / 50%

### Pillar blocks
1. Named regions structure the world
2. Discoveries are tracked and rewarded
3. Progression is tied to exploration

### Surface
- parchment background
- dark text
- creates a tonal shift from previous dark sections

---

## 8.3 Mobile Layout

### Stack order
1. section heading
2. intro paragraph
3. concept pillar blocks
4. key line / pull quote

Alternative:
pull quote can sit immediately after intro if it feels stronger.

---

## 9. The Experience Section

## 9.1 Purpose
Show the gameplay loop as a sequence, not a list of features.

## 9.2 Desktop Layout

### Recommended pattern
**Horizontal journey strip** or **stepped timeline**

Preferred version:
- horizontal 7-step sequence
- steps grouped into a guided path
- subtle directional flow across the section

### Structure
- section heading and intro above
- sequence below
- optional micro-caption under sequence

### Sequence item structure
Each step contains:
- number
- short title
- one-line explanation

### Desktop behavior
- can use 7 cards in a horizontal rail with wrap into 4+3
or
- 7 nodes in a connected timeline

### Best compromise
Use **card-based step grid with visible progression markers**:
- row 1: steps 1–4
- row 2: steps 5–7
This is easier to implement and more robust than a fancy timeline.

---

## 9.3 Mobile Layout

### Pattern
Vertical timeline

#### Stack
- steps in a single column
- numbers aligned left
- connecting line optional
- each step becomes its own readable block

### Priority
Readability over cleverness

---

## 9.4 Section Surface
- dark
- can include very subtle map line texture in background
- avoid heavy illustration behind the sequence

---

## 10. Core Systems Section

## 10.1 Purpose
Summarise systems clearly after the player understands the loop.

## 10.2 Desktop Layout

### Pattern
**2x2 feature grid**

Cards:
1. Named World
2. Discovery Progression
3. Meaningful Rewards
4. Persistent World

### Grid behavior
- desktop: 2 columns × 2 rows
- tablet: 2 columns
- mobile: 1 column

### Card contents
- short title
- 1–2 sentence explanation
- optional thin line icon

### Card height
Cards should align in height per row on desktop.

---

## 10.3 Section Width
- cards can sit within 1000px container for tighter composition
- do not stretch feature cards edge to edge unnecessarily

---

## 11. Exploration Servers Section

## 11.1 Purpose
Convert concept interest into actionable server choices.

## 11.2 Section Placement
This section should come only after the concept and loop are understood.

## 11.3 Desktop Layout

### Pattern
Intro band + card grid

#### Intro band
- section title
- one short paragraph
- optional filter or future placeholder for filtering

#### Card grid
- desktop: 2 or 3 columns depending on number of servers
- if only 1 server at launch, use a **featured wide card** rather than a lonely narrow card

### Recommended launch behavior
If only Charidh exists:
- use one large featured card with richer content
- optionally add “more servers coming” secondary block

### When multiple servers exist
Use responsive grid:
- 3 columns at wide desktop
- 2 columns at standard desktop
- 1 column at mobile

---

## 11.4 Server Card Structure

Each card should include:
- server name
- short descriptor
- key stats row
- server status
- version / access info
- primary CTA
- optional secondary CTA

### Example card hierarchy
1. Name
2. One-sentence description
3. Stat chips or inline stats
4. Status line
5. CTA row

### Stats presentation
Use either:
- inline stat row: `30 Regions · 56 Villages · 140+ Structures`
or
- 3 small chips

### Status presentation
- Online / Offline / Updating
- Keep subtle, not huge “live dashboard” styling

---

## 11.5 Mobile Server Cards

- single-column stack
- full-width buttons
- stats can wrap cleanly
- status should remain near top or just above CTA row

---

## 11.6 Surface
- parchment section strongly recommended
- dark text on light background helps the server cards feel like destination listings

---

## 12. Why This Exists Section

## 12.1 Purpose
Provide a concise philosophical landing after the mechanical explanation.

## 12.2 Layout

### Desktop
- narrow centered editorial block
- max width 640px
- generous whitespace around it

### Mobile
- same content, left-aligned or centered depending on readability
- prefer left-aligned if surrounding page text is mostly left-aligned

### Surface
- parchment or soft neutral
- should feel quieter than previous sections

### Content pattern
- short heading
- 2–3 short lines
- no CTA inside this block

---

## 13. Final CTA Section

## 13.1 Purpose
End with a simple, strong action.

## 13.2 Layout

### Desktop
Centered or left-aligned block within dark section.

Recommended structure:
- short heading
- one sentence
- button row

### CTA row
- Primary: View Servers
- Secondary: Join Discord

### Width
- 640–760px max

### Surface
- dark
- high contrast
- slightly stronger visual emphasis than mid-page sections

---

## 14. Footer

## 14.1 Layout

### Desktop
Three or four lightweight columns:
1. wordmark / descriptor
2. site nav
3. servers
4. community / Discord

### Mobile
Single-column stacked footer groups

### Footer content
Keep concise:
- brand / concept name
- quick nav
- servers
- Discord
- optional small note

---

## 15. Scroll & Sticky Behaviour

## 15.1 Sticky Header
Recommended.

### Behavior
- transparent over hero
- becomes solid/semi-opaque after first scroll threshold
- remains compact

## 15.2 Anchor Navigation
“How It Works” and “Servers” should scroll to section anchors.

## 15.3 Scroll rhythm
Avoid too many sticky internal elements.
Only the top header should be sticky at this stage.

## 15.4 Section reveal animations
Optional and subtle:
- fade-up on cards
- slight translate + opacity
- 150–220ms
No theatrical motion.

---

## 16. Responsive Priority Summary

## Desktop
- split hero
- 3-card problem row
- 2-column concept explainer
- structured experience sequence
- 2x2 systems grid
- 2–3 column server cards

## Tablet
- preserve structure where possible
- reduce visual density
- collapse some two-column sections earlier if spacing gets tight

## Mobile
- stack everything vertically
- maintain CTA prominence
- reduce decorative visuals
- keep cards readable and padded
- convert any multi-step horizontal logic into vertical flow

---

## 17. Section-by-Section Surface Map

| Section | Surface | Layout Pattern |
|---|---|---|
| Header | transparent → dark on scroll | fixed/sticky bar |
| Hero | dark | split column desktop / stacked mobile |
| The Shift | dark | 3-card row + closing line |
| What This Changes | parchment | 2-column explainer |
| The Experience | dark | timeline / progression grid |
| Core Systems | dark | 2x2 card grid |
| Exploration Servers | parchment | intro + responsive card grid |
| Why This Exists | parchment/soft | narrow editorial block |
| Final CTA | dark | focused closing band |
| Footer | dark | simple multi-column / stacked |

---

## 18. Launch Recommendation

For v1, keep the page to a single homepage with these sections only.

Do not add, at launch:
- testimonial sliders
- screenshots carousel overload
- plugin breakdowns
- news feed
- blog system
- overly detailed filtering
- world maps as interactive widgets unless they are high quality

The structural priority is clarity, not quantity.

---

## 19. Build Handoff Notes

This wireframe should translate naturally into Tailwind with:
- a 1200px container
- clear section wrappers
- responsive grid utilities
- alternating surface sections
- sticky nav
- reusable card patterns

### Suggested implementation pieces
- `SiteHeader`
- `HeroSection`
- `ProblemSection`
- `ConceptSection`
- `ExperienceSection`
- `SystemsGrid`
- `ServersSection`
- `WhyExistsSection`
- `FinalCTA`
- `SiteFooter`

---

## 20. Final Standard

A correct implementation of this wireframe should make the user feel:

- this is different from a normal SMP
- this has a clear exploration loop
- the world itself is part of progression
- there is somewhere concrete to go next

If the page feels like a generic Minecraft server landing page, the wireframe has not been implemented correctly.

# Exploration Servers – Design Token System

A Tailwind-oriented visual system for a cartographic, atlas-inspired promotional website.

---

## Design Intent
The site should feel like a **world interface**, not a SaaS dashboard.  
The visual language should evoke maps, travel journals, and a sense of place while remaining modern, readable, and restrained.

---

## 1. Core Principles

- **World, not product:** The UI should support the feeling of uncovering a place rather than using an app.  
- **Editorial, not dashboard:** Prioritise reading flow, hierarchy, and section pacing over widget-heavy layouts.  
- **Grounded, not flashy:** Use muted earth tones, subtle surfaces, and calm motion instead of neon or heavy effects.  
- **Readable first:** Body text, labels, cards, and calls to action must remain crisp and easy to scan.  

---

## 2. Typography Tokens

Recommended pairing: serif for narrative, sans-serif for UI.

| Token            | Font              | Size / Line Height | Use                          |
|------------------|-------------------|--------------------|-------------------------------|
| Display / Hero   | Playfair Display  | 44 / 1.05          | Hero headings                 |
| Section Title    | Playfair Display  | 28 / 1.15          | Section headings              |
| Subheading       | Inter             | 20 / 1.2           | Card headings                 |
| Body             | Inter             | 16 / 1.6           | Body copy                     |
| Small UI         | Inter             | 14 / 1.45          | Labels, metadata              |
| Button / Nav     | Inter             | 15 / 1.2           | Navigation, CTA               |

---

## 3. Colour Tokens

| Token             | Hex       | Purpose                     | Tone         |
|-------------------|-----------|-----------------------------|--------------|
| bg.base           | #0F172A   | Main background             | Deep slate   |
| bg.surface        | #1E293B   | Cards / panels              | Soft slate   |
| bg.soft           | #F8F5EE   | Light sections              | Parchment    |
| text.strong       | #243447   | Headings                    | Ink slate    |
| text.body         | #374151   | Body text                   | Muted ink    |
| text.subtle       | #6B7280   | Metadata                    | Low emphasis |
| accent.earth      | #8B7355   | Primary accent              | Bronze       |
| accent.parchment  | #C2A878   | Highlight                   | Warm gold    |
| accent.moss       | #3E5C47   | Secondary accent            | Moss green   |
| border.soft       | #D7D3CB   | Borders                     | Neutral      |

---

## 4. Spacing & Radius

| Token       | Value | Use                      |
|------------|------|--------------------------|
| space.1    | 4px  | Fine spacing             |
| space.2    | 8px  | Tight spacing            |
| space.3    | 12px | Compact layouts          |
| space.4    | 16px | Default padding          |
| space.6    | 24px | Section clusters         |
| space.8    | 32px | Card padding             |
| space.12   | 48px | Section separation       |
| space.16   | 64px | Large sections           |

| Token       | Value |
|------------|------|
| radius.md  | 12px |
| radius.lg  | 18px |
| radius.xl  | 24px |

---

## 5. Layout Tokens

| Token              | Value                         |
|--------------------|-------------------------------|
| container.max      | 1200px                        |
| container.reading  | 760px                         |
| grid.serverCards   | auto-fit minmax(320px, 1fr)   |
| section.padY       | 96 / 72 / 56 responsive       |

---

## 6. Components

- **Primary Button:** accent.earth background, light text  
- **Secondary Button:** border-only  
- **Cards:** soft surface + subtle border  
- **Editorial Blocks:** parchment background  

---

## 7. Motion & Accessibility

- 150–220ms transitions  
- No heavy animation  
- WCAG AA contrast minimum  
- Visible focus states  

---

## 8. Tailwind Mapping

```js
theme: {
  extend: {
    colors: {
      bg: { base: '#0F172A', surface: '#1E293B', soft: '#F8F5EE' },
      text: { strong: '#243447', body: '#374151', subtle: '#6B7280' },
      accent: { earth: '#8B7355', parchment: '#C2A878', moss: '#3E5C47' },
      border: { soft: '#D7D3CB' },
    },
    fontFamily: {
      display: ['Playfair Display', 'serif'],
      body: ['Inter', 'sans-serif'],
    },
  }
}
```

---

## 9. Usage Guidance

- Use serif sparingly for emphasis  
- Keep UI clean and readable  
- Avoid SaaS-style layouts  
- Prioritise world-building feel over UI complexity  

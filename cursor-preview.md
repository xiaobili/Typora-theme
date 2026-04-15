# Cursor Theme Preview

## Typography Showcase

### Heading Level 1 (72px, -2.16px spacing)

This is a demonstration of the Cursor theme's typography system. The heading above uses aggressive negative letter-spacing to create that compressed, engineered feel characteristic of CursorGothic.

### Heading Level 2 (36px, -0.72px spacing)

Body text uses jjannon serif font with contextual swash alternates enabled, providing a literary warmth that contrasts beautifully with the gothic headings. The warm cream background (`#f2f1ed` in light mode, `#1a1915` in dark mode) creates an organic, paper-like reading experience.

### Heading Level 3 (26px, -0.325px spacing)

The progressive reduction in letter-spacing as heading sizes decrease creates a natural visual hierarchy. This is paragraph text demonstrating the body typography at 17.28px with 1.5 line height.

#### Heading Level 4 (22px, -0.11px spacing)

At this size, the letter-spacing is nearly normal, creating a subtle transition from display typography to functional UI text. The three-font system (gothic, serif, mono) provides distinct voices for different content types.

##### Heading Level 5 (18px, normal spacing)

Smaller headings maintain readability while continuing the typographic scale. Notice how the warm color palette avoids cold grays entirely.

###### Heading Level 6 (16px, normal spacing)

The smallest heading size serves as section markers and metadata labels throughout documents.

---

## Text Formatting

This is **bold text** using weight 500 for emphasis without being too heavy. This is *italic text* with a subtle warmth. This is ***bold italic*** combining both styles.

Here's some `inline code` using berkeleyMono at 12px with warm surface backgrounds. You can also ~~strikethrough~~ text for deletions.

> This is a blockquote with jjannon serif font and orange left border. Blockquotes use the warm surface color (`#ebeae5` in light mode) and feature the signature 3px border in accent orange (`#f54e00`). The text color is softened to 55% opacity for secondary emphasis.

## Lists

### Unordered List

- First item with serif body text
- Second item demonstrating list spacing
  - Nested item with proper indentation
  - Another nested item
    - Third level nesting maintains clarity
- Back to first level

### Ordered List

1. First ordered item (Arabic numerals)
2. Second item showing standard numbering
   i. Nested with Roman numerals
   ii. Second Roman numeral item
      a. Third level uses letters
      b. Continuing alphabetic sequence
3. Back to Arabic numerals

### Task List

- [x] Completed task with accent orange checkbox
- [ ] Pending task ready for action
- [x] Another completed item
- [ ] Final pending task

## Code Blocks

```javascript
// JavaScript example with berkeleyMono font
function calculateSpacing(base = 8) {
  const scale = {
    micro: base * 0.1875,  // 1.5px
    small: base * 0.25,    // 2px
    medium: base * 0.3125, // 2.5px
    base: base,            // 8px
    large: base * 1.25,    // 10px
    xl: base * 1.5,        // 12px
  };
  
  return scale;
}

const spacing = calculateSpacing();
console.log(`Base spacing: ${spacing.base}px`);
```

```python
# Python example showing syntax highlighting
class CursorTheme:
    def __init__(self):
        self.background = "#f2f1ed"  # Warm cream
        self.text = "#26251e"        # Warm near-black
        self.accent = "#f54e00"      # Orange
    
    def apply_typography(self, element):
        if element.type == "heading":
            return {
                "font": "CursorGothic",
                "spacing": self.calculate_spacing(element.level)
            }
        return {"font": "jjannon"}
    
    def calculate_spacing(self, level):
        # Progressive letter-spacing reduction
        spacing_map = {
            1: -2.16,
            2: -0.72,
            3: -0.325,
            4: -0.11,
        }
        return spacing_map.get(level, 0)
```

```css
/* CSS example showing theme variables */
:root {
  --cursor-dark: #26251e;
  --cursor-cream: #f2f1ed;
  --cursor-orange: #f54e00;
  --error-warm: #cf2d56;
  
  /* Spacing with fine increments */
  --space-1: 1.5px;
  --space-2: 2px;
  --space-base: 8px;
  --space-3xl: 24px;
}
```

## Tables

| Feature | Light Theme | Dark Theme | Notes |
|---------|-------------|------------|-------|
| Background | `#f2f1ed` | `#1a1915` | Warm tones only |
| Text Color | `#26251e` | `#e6e5e0` | Never pure black/white |
| Accent | `#f54e00` | `#f54e00` | Consistent orange |
| Hover State | `#cf2d56` | `#cf2d56` | Warm crimson |
| Border Alpha | `0.1` | `0.1` | Perceptually uniform |
| Shadow Blur | 28px, 70px | 28px, 70px | Atmospheric depth |

Table rows have hover effects that shift to slightly warmer surface tones, maintaining the organic feel of the design system.

## Images

![Placeholder Image](https://via.placeholder.com/800x400/ebeae5/26251e?text=Cursor+Theme+Preview)

*Image caption using jjannon serif in italic style with warm gray color*

## Horizontal Rules

The horizontal rule above uses a subtle warm border (`rgba(38, 37, 30, 0.1)`) rather than a harsh line, maintaining the organic aesthetic throughout.

---

## Special Elements

### Footnotes

Here's a sentence with a footnote reference[^1]. This demonstrates how footnotes appear at the bottom of the document with proper styling.

### Math Equations

When $x = 42$, the equation $E = mc^2$ demonstrates inline math. Display math appears centered:

$$\int_{0}^{\infty} e^{-x^2} dx = \frac{\sqrt{\pi}}{2}$$

### Front Matter

```yaml
---
title: Cursor Theme Demo
author: Theme Generator
date: 2026-04-15
tags: [typora, cursor, theme]
---
```

## Responsive Behavior

The theme adapts gracefully across screen sizes:

- **Desktop (>1279px)**: Full layout with maximum 1200px content width
- **Tablet (768-1279px)**: Adjusted spacing and heading sizes
- **Mobile (<768px)**: Single column, reduced padding, stacked elements

Heading sizes scale down proportionally on smaller screens while maintaining the letter-spacing ratios.

## Color Palette Reference

### Light Theme Surfaces
- Surface 100: `#f7f7f4` (lightest)
- Surface 200: `#f2f1ed` (page background)
- Surface 300: `#ebeae5` (buttons, cards)
- Surface 400: `#e6e5e0` (secondary surfaces)
- Surface 500: `#e1e0db` (tertiary emphasis)

### Dark Theme Surfaces
- Surface 100: `#2a2925` (darkest surface)
- Surface 200: `#1a1915` (page background)
- Surface 300: `#262520` (cards, code blocks)
- Surface 400: `#2a2925` (tables, containers)
- Surface 500: `#2e2d28` (emphasis surfaces)

### Semantic Colors
- **Accent Orange**: `#f54e00` - Primary brand color, links, CTAs
- **Error/Hover**: `#cf2d56` - Warm crimson for interactive states
- **Success**: `#1f8a65` - Muted teal-green
- **Gold**: `#c08532` - Secondary accent for premium contexts

---

[^1]: This is the footnote text. It appears at the bottom of the document with smaller font size (14px) and softer color (55% opacity).

---

**End of Preview** - This document demonstrates all major elements of the Cursor themes for Typora. Switch between Cursor Light and Cursor Dark to see both variations!

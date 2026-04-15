# Cursor Themes - Quick Reference

## 🎨 Color Values

### Light Theme
```css
Background:    #f2f1ed  /* Warm cream */
Text Primary:  #26251e  /* Warm near-black */
Text Secondary: rgba(38, 37, 30, 0.55)
Accent Orange: #f54e00
Hover Crimson: #cf2d56
Success Teal:  #1f8a65

Surfaces:
  100: #f7f7f4
  200: #f2f1ed  (page bg)
  300: #ebeae5  (buttons/cards)
  400: #e6e5e0
  500: #e1e0db

Borders:
  Primary:   rgba(38, 37, 30, 0.1)
  Medium:    rgba(38, 37, 30, 0.2)
  Strong:    rgba(38, 37, 30, 0.55)
```

### Dark Theme
```css
Background:    #1a1915  /* Deep warm brown */
Text Primary:  #e6e5e0  /* Warm off-white */
Text Secondary: rgba(230, 229, 224, 0.6)
Accent Orange: #f54e00  /* Same as light */
Hover Crimson: #cf2d56  /* Same as light */
Success Teal:  #1f8a65  /* Same as light */

Surfaces:
  100: #2a2925
  200: #1a1915  (page bg)
  300: #262520  (cards/code)
  400: #2a2925  (tables)
  500: #2e2d28

Borders:
  Primary:   rgba(230, 229, 224, 0.1)
  Medium:    rgba(230, 229, 224, 0.2)
  Strong:    rgba(230, 229, 224, 0.55)
```

## 📏 Typography

### Headings (CursorGothic)
```css
H1: 72px,  weight 400, line-height 1.1,  letter-spacing -2.16px
H2: 36px,  weight 400, line-height 1.2,  letter-spacing -0.72px
H3: 26px,  weight 400, line-height 1.25, letter-spacing -0.325px
H4: 22px,  weight 400, line-height 1.3,  letter-spacing -0.11px
H5: 18px,  weight 400, line-height 1.35, letter-spacing normal
H6: 16px,  weight 400, line-height 1.4,  letter-spacing normal
```

### Body & Code
```css
Body: 17.28px, jjannon serif, line-height 1.5, font-feature-settings: "cswh"
Lead: 19.2px,  jjannon serif, line-height 1.5
Code: 12px,    berkeleyMono, line-height 1.67
```

## 📐 Spacing Scale

```css
Micro:     1.5px, 2px, 2.5px, 3px
Standard:  4px, 5px, 6px, 8px (base)
Extended:  10px, 12px, 16px, 24px, 32px, 48px, 64px, 80px, 96px

Common Usage:
  --space-base:   8px   (component padding)
  --space-2xl:    16px  (paragraph margin)
  --space-3xl:    24px  (section spacing)
  --space-4xl:    32px  (large padding)
  --space-5xl:    48px  (major sections)
  --space-7xl:    80px  (hero/top padding)
```

## 🔲 Border Radius

```css
Micro:      1.5px
Small:      2px     (inline code)
Medium:     3px
Standard:   4px     (compact elements)
Comfortable: 8px    (buttons, cards, primary)
Featured:   10px    (larger containers)
Pill:       9999px  (tags, filters, pills)
```

## 🌊 Shadows

### Light Theme
```css
Card Shadow:
  rgba(0,0,0,0.14) 0px 28px 70px,
  rgba(0,0,0,0.1) 0px 14px 32px,
  rgba(38,37,30,0.1) 0px 0px 0px 1px

Ambient Shadow:
  rgba(0,0,0,0.02) 0px 0px 16px,
  rgba(0,0,0,0.008) 0px 0px 8px

Focus Shadow:
  rgba(0,0,0,0.1) 0px 4px 12px
```

### Dark Theme
```css
Card Shadow:
  rgba(0,0,0,0.3) 0px 28px 70px,
  rgba(0,0,0,0.2) 0px 14px 32px,
  rgba(230,229,224,0.1) 0px 0px 0px 1px

Ambient Shadow:
  rgba(0,0,0,0.05) 0px 0px 16px,
  rgba(0,0,0,0.02) 0px 0px 8px

Focus Shadow:
  rgba(0,0,0,0.3) 0px 4px 12px
```

## 🎯 Component Styles

### Buttons
```css
Primary Button:
  bg: var(--surface-300)
  text: var(--cursor-dark)
  radius: 8px
  padding: 10px 12px 10px 14px
  hover: text → var(--error-warm)

Pill Button:
  bg: var(--surface-400)
  text: rgba(dark, 0.6)
  radius: 9999px
  padding: 3px 8px
  hover: text → var(--error-warm)
```

### Blockquotes
```css
Font: jjannon serif, 17.28px
Border-left: 3px solid var(--cursor-orange)
Background: var(--surface-300)
Padding: 24px 32px
Radius: 0 8px 8px 0
Color: rgba(dark, 0.55)
```

### Code Blocks
```css
Font: berkeleyMono, 12px
Background: var(--surface-300)
Border: 1px solid var(--border-primary)
Radius: 8px
Padding: 24px
Line-height: 1.67
```

### Tables
```css
Background: var(--surface-400)
Border: 1px solid var(--border-primary)
Radius: 8px

Header:
  bg: var(--surface-300)
  font: CursorGothic, 14px
  border-bottom: 2px solid var(--border-medium)

Cell:
  font: jjannon serif, 15px
  border-bottom: 1px solid var(--border-primary)
  
Hover:
  bg: var(--surface-300)
```

## 📱 Responsive Breakpoints

```css
Mobile:      < 600px   (single column, reduced spacing)
Tablet:      600-768px (2-column grids begin)
Desktop:     > 768px   (full layout)
Large:       > 1279px  (max content width 1200px)

Heading Scaling:
  H1: 72px → 36px → 28px
  H2: 36px → 26px → 22px
  H3: 26px → 22px → 18px
```

## 🔗 Interactive States

### Links
```css
Default:
  color: var(--cursor-dark)
  border-bottom: 1px solid var(--border-primary)
  
Hover:
  color: var(--cursor-orange)
  border-bottom-color: var(--cursor-orange)
  transition: 150ms ease
```

### Buttons
```css
Hover:
  color: var(--error-warm)  /* #cf2d56 */
  box-shadow: var(--shadow-focus)
  transition: 150ms ease
```

### Cards/Tables
```css
Hover:
  background: var(--surface-300)
  transition: 200ms ease
```

## 🎨 Timeline Colors

Used for AI operation indicators:
```css
Thinking: #dfa88f  /* Warm peach */
Grep:     #9fc9a2  /* Soft sage */
Read:     #9fbbe0  /* Soft blue */
Edit:     #c0a8dd  /* Soft lavender */
```

## 💡 Quick Tips

1. **Never use pure black (#000000) or pure white (#ffffff)** for primary surfaces
2. **Always use warm tones** - the entire palette is warm-shifted
3. **Letter-spacing scales with size** for CursorGothic headings
4. **Use oklab/rgba borders** for perceptually uniform edges
5. **Shadows use large blur values** (28px, 70px) for atmospheric depth
6. **Three fonts, three voices**: Gothic (display), Serif (body), Mono (code)
7. **Pill shapes** (9999px radius) for tags; 8px for primary UI
8. **Hover states** shift to crimson (#cf2d56) - signature interaction

---

**Keep this reference handy while customizing your Cursor themes!**

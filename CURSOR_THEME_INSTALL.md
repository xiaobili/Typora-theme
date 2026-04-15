# Cursor Themes for Typora - Installation Guide

## Overview

Two elegant Typora themes inspired by [Cursor's](https://cursor.sh) design system:

- **Cursor Light**: Warm cream tones with gothic typography
- **Cursor Dark**: Deep warm tones with atmospheric depth

Both themes feature:
- Progressive letter-spacing on headings (CursorGothic style)
- Three-font system: Gothic (headings), Serif (body), Mono (code)
- Warm color palette avoiding cold grays
- Pill-shaped elements and organic borders
- Responsive design for all screen sizes

## Installation

### Method 1: Manual Installation

1. **Download the theme files**:
   - For light theme: `cursor-light.css`
   - For dark theme: `cursor-dark.css`

2. **Open Typora's theme folder**:
   - Open Typora
   - Go to **Preferences** → **Appearance**
   - Click **Open Theme Folder**

3. **Copy the CSS file(s)**:
   - Copy `cursor-light.css` and/or `cursor-dark.css` to the theme folder
   - Optionally copy the corresponding `package-cursor-*.json` files (rename to `package.json` if you want metadata)

4. **Restart Typora**

5. **Select the theme**:
   - Go to **Preferences** → **Appearance** → **Themes**
   - Select "Cursor Light" or "Cursor Dark"

### Method 2: Using Both Themes

You can install both themes and switch between them:
- Install both `cursor-light.css` and `cursor-dark.css`
- They will appear as separate themes in Typora
- Switch based on your preference or time of day

## Features

### Typography

**Headings** (CursorGothic style):
- H1: 72px, letter-spacing: -2.16px
- H2: 36px, letter-spacing: -0.72px
- H3: 26px, letter-spacing: -0.325px
- H4: 22px, letter-spacing: -0.11px
- H5-H6: Normal spacing

**Body Text** (jjannon serif):
- Size: 17.28px
- Line height: 1.5
- OpenType feature: contextual swash alternates ("cswh")

**Code** (berkeleyMono):
- Size: 12px
- Line height: 1.67
- Monospace for technical content

### Color Palette

#### Light Theme
- Background: `#f2f1ed` (warm cream)
- Text: `#26251e` (warm near-black)
- Accent: `#f54e00` (orange)
- Hover: `#cf2d56` (warm crimson)
- Surfaces: Scale from `#f7f7f4` to `#e1e0db`

#### Dark Theme
- Background: `#1a1915` (deep warm brown)
- Text: `#e6e5e0` (warm off-white)
- Accent: `#f54e00` (orange - same as light)
- Hover: `#cf2d56` (warm crimson - same as light)
- Surfaces: Scale from `#2a2925` to `#2e2d28`

### Design Elements

- **Borders**: Perceptually uniform using rgba with alpha values
- **Shadows**: Large blur values (28px, 70px) for atmospheric depth
- **Border Radius**: 
  - Standard: 8px (cards, buttons)
  - Pills: 9999px (tags, filters)
- **Spacing**: 8px base system with fine sub-8px increments (1.5px, 2px, 2.5px, etc.)

## Customization

### Changing Fonts

If you don't have CursorGothic, jjannon, or berkeleyMono installed, the themes will fall back to system fonts. To use custom fonts:

1. Install the fonts on your system
2. The CSS already includes fallback chains
3. Or edit the CSS variables in the `:root` section:

```css
--font-gothic: "Your Preferred Font", system-ui, sans-serif;
--font-serif: "Your Preferred Serif", Georgia, serif;
--font-mono: "Your Preferred Mono", monospace;
```

### Adjusting Colors

Edit the CSS variables in the `:root` section of either theme file:

```css
:root {
  --cursor-orange: #f54e00;  /* Change accent color */
  --error-warm: #cf2d56;     /* Change hover color */
  /* ... other variables ... */
}
```

### Modifying Spacing

Adjust the spacing scale if needed:

```css
:root {
  --space-base: 8px;    /* Base unit */
  --space-3xl: 24px;    /* Section spacing */
  /* ... other spacing variables ... */
}
```

## Troubleshooting

### Theme not appearing in Typora

1. Ensure the CSS file is in the correct theme folder
2. Check that the filename ends with `.css`
3. Restart Typora completely
4. Verify file permissions (should be readable)

### Fonts not displaying correctly

1. The themes use fallback fonts if CursorGothic/jjannon/berkeleyMono aren't installed
2. Install the fonts for the authentic Cursor experience
3. Or customize the font variables to use fonts you have

### Dark mode not switching automatically

The themes include media query support for automatic switching. If it's not working:
1. Check your OS dark mode settings
2. Manually select the desired theme in Typora preferences
3. Each theme also includes optional override queries

## Credits

- **Design Inspiration**: [Cursor](https://cursor.sh) - The AI-first code editor
- **Typography**: CursorGothic, jjannon, berkeleyMono (Cursor's custom fonts)
- **Color System**: Warm-toned palette avoiding cold grays
- **Implementation**: Adapted for Typora's markdown rendering engine

## License

This theme is inspired by Cursor's design system. The original design belongs to Cursor. This implementation is for personal use and follows fair use principles for design inspiration.

## Support

For issues or questions:
1. Check this installation guide
2. Review the CSS comments for customization options
3. Refer to Typora's official documentation for theme-related features

---

**Enjoy writing with Cursor themes!** ✨

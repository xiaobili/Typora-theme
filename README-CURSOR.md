# Cursor Themes for Typora

Elegant Typora themes inspired by [Cursor's](https://cursor.sh) design system, featuring warm minimalism, gothic typography, and organic depth.

![Preview](cursor-preview.md)

## 🎨 Themes Included

### Cursor Light
A warm, minimalist theme with cream tones and compressed gothic headings. Perfect for daytime writing with reduced eye strain.

**Key Features:**
- Background: Warm cream (`#f2f1ed`)
- Text: Warm near-black (`#26251e`)
- Typography: Progressive letter-spacing on headings
- Accent: Vibrant orange (`#f54e00`)

### Cursor Dark
A deep, atmospheric theme with warm brown tones and diffused shadows. Ideal for evening coding sessions.

**Key Features:**
- Background: Deep warm brown (`#1a1915`)
- Text: Warm off-white (`#e6e5e0`)
- Shadows: Large blur values for atmospheric depth
- Accent: Same vibrant orange for consistency

## ✨ Design Philosophy

### Warm Minimalism
Unlike cold, clinical dark themes, Cursor themes use exclusively warm tones throughout the entire color palette. No pure blacks, no cold grays - just organic warmth reminiscent of old paper and ink.

### Three-Voice Typography
- **CursorGothic** (Display/UI): Aggressive negative letter-spacing creates compressed, engineered headlines
- **jjannon** (Body/Editorial): Serif font with contextual swash alternates for literary warmth
- **berkeleyMono** (Code): Refined monospace connecting to Cursor's code editor identity

### Perceptually Uniform Borders
Borders use rgba with alpha values (0.1, 0.2, 0.55) rather than solid colors, creating organic edges that feel like they're part of the page rather than drawn on top.

### Atmospheric Depth
Shadows use dramatically large blur values (28px, 70px) with moderate opacity, creating diffused elevation that feels like the page has gently opened a space for elements.

## 🚀 Quick Start

### Installation

1. **Download** `cursor-light.css` or `cursor-dark.css` (or both!)
2. **Open Typora** → Preferences → Appearance → Open Theme Folder
3. **Copy** the CSS file(s) to the theme folder
4. **Restart** Typora
5. **Select** "Cursor Light" or "Cursor Dark" from the theme menu

See [CURSOR_THEME_INSTALL.md](CURSOR_THEME_INSTALL.md) for detailed installation instructions.

### Preview

Open `cursor-preview.md` in Typora with either theme activated to see all elements styled beautifully.

## 📐 Design System

### Typography Scale

| Element | Size | Letter Spacing | Font |
|---------|------|----------------|------|
| H1 | 72px | -2.16px | CursorGothic |
| H2 | 36px | -0.72px | CursorGothic |
| H3 | 26px | -0.325px | CursorGothic |
| H4 | 22px | -0.11px | CursorGothic |
| Body | 17.28px | normal | jjannon serif |
| Code | 12px | normal | berkeleyMono |

### Spacing System

Base unit: 8px with fine sub-8px increments:
- Micro: 1.5px, 2px, 2.5px, 3px
- Standard: 4px, 5px, 6px, 8px
- Extended: 10px, 12px, 16px, 24px, 32px, 48px, 64px, 80px, 96px

### Border Radius

- Micro: 1.5px
- Small: 2px
- Medium: 3px
- Standard: 4px
- Comfortable: 8px (primary buttons, cards)
- Featured: 10px
- Pill: 9999px (tags, filters)

### Color Palette

#### Light Theme
```
Background: #f2f1ed (warm cream)
Text:       #26251e (warm near-black)
Accent:     #f54e00 (orange)
Hover:      #cf2d56 (warm crimson)
Surfaces:   #f7f7f4 → #e1e0db (5-step scale)
```

#### Dark Theme
```
Background: #1a1915 (deep warm brown)
Text:       #e6e5e0 (warm off-white)
Accent:     #f54e00 (orange - same as light)
Hover:      #cf2d56 (warm crimson - same as light)
Surfaces:   #2a2925 → #2e2d28 (5-step scale)
```

## 🎯 Key Components

### Headings
Progressive letter-spacing creates visual compression at larger sizes, gradually relaxing as sizes decrease. This mimics the precision engineering aesthetic of Cursor's brand.

### Code Blocks
Warm surface backgrounds (`#ebeae5` light / `#262520` dark) with berkeleyMono font create a cohesive coding experience that connects to Cursor's core identity.

### Blockquotes
Orange left border (3px) with warm surface background and jjannon serif font creates distinctive callout sections perfect for quotes and important notes.

### Tables
Clean borders with hover effects that shift surface tones subtly. Headers use gothic font while body uses serif for clear hierarchy.

### Buttons
- **Primary**: Warm surface background, hover shifts text to crimson
- **Pill**: Full-radius (9999px) for tags and filters
- **Ghost**: Transparent with subtle background tint

## 🔧 Customization

### Change Fonts
Edit CSS variables in the `:root` section:
```css
--font-gothic: "Your Font", system-ui, sans-serif;
--font-serif: "Your Serif", Georgia, serif;
--font-mono: "Your Mono", monospace;
```

### Adjust Colors
Modify any color variable:
```css
--cursor-orange: #your-color;
--error-warm: #your-hover-color;
```

### Modify Spacing
Tweak the spacing scale:
```css
--space-base: 8px;
--space-3xl: 24px;
```

See [CURSOR_THEME_INSTALL.md](CURSOR_THEME_INSTALL.md) for full customization guide.

## 📱 Responsive Design

Both themes adapt gracefully across devices:

- **Desktop**: Full layout, maximum 1200px content width
- **Tablet**: Adjusted spacing, 2-column grids where applicable
- **Mobile**: Single column, reduced padding, stacked navigation

Heading sizes scale proportionally while maintaining letter-spacing ratios.

## 🌗 Dark Mode Support

Both themes include media query support for automatic switching based on OS preferences:
- `cursor-light.css`: Includes dark mode override
- `cursor-dark.css`: Includes light mode override

You can also manually select your preferred theme regardless of OS settings.

## 📄 File Structure

```
Typora-theme/
├── cursor-light.css           # Light theme stylesheet
├── cursor-dark.css            # Dark theme stylesheet
├── package-cursor-light.json  # Light theme metadata
├── package-cursor-dark.json   # Dark theme metadata
├── cursor-preview.md          # Preview document
├── CURSOR_THEME_INSTALL.md    # Installation guide
└── README-CURSOR.md           # This file
```

## 🙏 Credits

- **Design Inspiration**: [Cursor](https://cursor.sh) - The AI-first code editor
- **Typography**: CursorGothic, jjannon, berkeleyMono (Cursor's custom typefaces)
- **Color System**: Warm-toned palette avoiding cold grays entirely
- **Implementation**: Adapted for Typora's markdown rendering engine

## 📝 License

This theme is inspired by Cursor's design system. The original design belongs to Cursor. This implementation is for personal use and follows fair use principles for design inspiration.

The CSS code and implementation details are free to use and modify for personal projects.

## 🐛 Troubleshooting

### Theme not appearing?
1. Verify CSS file is in Typora's theme folder
2. Check filename ends with `.css`
3. Restart Typora completely
4. Verify file permissions

### Fonts not displaying?
- Themes include fallback chains for system fonts
- Install CursorGothic/jjannon/berkeleyMono for authentic experience
- Or customize font variables to use fonts you have

### Need help?
1. Review [CURSOR_THEME_INSTALL.md](CURSOR_THEME_INSTALL.md)
2. Check CSS comments for customization options
3. Refer to Typora's official documentation

## 🎉 Enjoy Writing!

Experience the warmth and elegance of Cursor's design system in your markdown documents. Whether you're writing technical documentation, creative prose, or daily notes, these themes provide a beautiful, comfortable reading and writing environment.

---

**Made with ❤️ for the Typora community**

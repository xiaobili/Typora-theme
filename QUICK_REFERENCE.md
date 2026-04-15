# Claude Anthropic Theme - Quick Reference Card

## 🎨 Color Palette 色彩速查

### Primary Colors 主色
```
Near Black:     #141413  (主要文字/深色背景)
Terracotta:     #c96442  (品牌强调色/CTA)
Coral Accent:   #d97757  (次要强调)
```

### Backgrounds 背景色
```
Parchment:      #f5f4ed  (页面主背景)
Ivory:          #faf9f5  (卡片/容器)
Pure White:     #ffffff  (按钮表面)
Warm Sand:      #e8e6dc  (按钮背景)
Dark Surface:   #30302e  (深色主题表面)
```

### Text Colors 文字颜色
```
Primary:        #141413  (主要文字)
Secondary:      #5e5d59  (次要文字)
Tertiary:       #87867f  (辅助文字)
Links:          #3d3d3a  (链接)
On Dark:        #b0aea5  (深色背景上的文字)
```

### Borders & Rings 边框
```
Border Cream:   #f0eee6  (浅色边框)
Border Warm:    #e8e6dc  (强调边框)
Ring Warm:      #d1cfc5  (交互环影)
Focus Blue:     #3898ec  (焦点环 - 唯一冷色)
```

---

## 📐 Typography Scale 排版比例

### Headings (All Serif, Weight 500)
```
H1:  64px  / 1.10 LH  (Display/Hero)
H2:  52px  / 1.20 LH  (Section)
H3:  36px  / 1.30 LH  (Sub-section)
H4:  32px  / 1.10 LH  (Card titles)
H5:  25px  / 1.20 LH  (Small sections)
H6:  20px  / 1.20 LH  (Minor headings)
```

### Body Text (Sans-serif)
```
Body Large:   20px  / 1.60 LH  (Intro paragraphs)
Body:         16px  / 1.60 LH  (Standard text)
Body Small:   15px  / 1.60 LH  (Compact text)
Caption:      14px  / 1.43 LH  (Metadata)
Label:        12px  / 1.25 LH  (Badges)
```

### Code (Monospace)
```
Code:         15px  / 1.60 LH  (Inline & blocks)
```

---

## 📏 Spacing System 间距系统

Base unit: **8px**

```
xs:    3px
sm:    4px
md:    6px
base:  8px    ← Base unit
lg:    10px
xl:    12px
2xl:   16px
3xl:   20px
4xl:   24px
5xl:   30px
```

### Common Usage
```
Button padding:      8px 16px (vertical horizontal)
Card padding:        24-32px internal
Section spacing:     80-120px vertical
Paragraph margin:    0 0 16px 0
List item margin:    8px bottom
```

---

## 🔲 Border Radius 圆角半径

```
Sharp:          4px    (Minimal inline elements)
Subtle:         6px    (Small buttons)
Comfortable:    8px    (Standard buttons, cards) ← Most common
Generous:       12px   (Primary buttons, inputs)
Very:           16px   (Featured containers, code blocks)
Highly:         24px   (Tags, highlights)
Maximum:        32px   (Hero containers, media)
```

---

## 🌟 Component Patterns 组件模式

### Buttons 按钮
```css
/* Secondary Button */
background: #e8e6dc;
color: #4d4c48;
padding: 8px 16px 8px 12px;
border-radius: 8px;
box-shadow: 0 0 0 1px #d1cfc5;

/* Primary CTA */
background: #c96442;
color: #faf9f5;
padding: 8px 16px 8px 12px;
border-radius: 12px;
box-shadow: 0 0 0 1px #c96442;
```

### Cards 卡片
```css
background: #faf9f5;
border: 1px solid #f0eee6;
border-radius: 8px;
padding: 24-32px;
box-shadow: rgba(0,0,0,0.05) 0px 4px 24px;
```

### Blockquotes 引用块
```css
font-family: Serif;
font-size: 17px;
line-height: 1.60;
border-left: 4px solid #c96442;
background: #faf9f5;
padding: 20px 24px;
border-radius: 0 8px 8px 0;
```

### Ordered Lists 有序列表
```css
/* Level 1: Arabic numerals */
ol { list-style-type: decimal; }        /* 1, 2, 3 */

/* Level 2: Roman numerals */
ol ol { list-style-type: lower-roman; } /* i, ii, iii */

/* Level 3: Letters */
ol ol ol { list-style-type: lower-alpha; } /* a, b, c */

/* Level 4+: Reset to Arabic */
ol ol ol ol { list-style-type: decimal; }
```

### Code Blocks 代码块
```css
background: #faf9f5;  /* Ivory - 象牙白 */
color: #4d4c48;       /* Charcoal Warm - 炭灰 */
padding: 24px;
border-radius: 16px;
border: 1px solid #f0eee6;  /* Border Cream - 奶油边 */
```

---

## ⚡ Shadow System 阴影系统

### Level 0: Flat
```css
/* No shadow, no border */
/* Use: Background, inline text */
```

### Level 1: Contained
```css
border: 1px solid #f0eee6;  /* Light theme */
border: 1px solid #30302e;  /* Dark theme */
/* Use: Standard cards, sections */
```

### Level 2: Ring
```css
box-shadow: 0 0 0 1px #d1cfc5;
/* Use: Interactive elements, hover states */
```

### Level 3: Whisper
```css
box-shadow: rgba(0,0,0,0.05) 0px 4px 24px;
/* Use: Elevated cards, screenshots */
```

### Level 4: Inset
```css
box-shadow: inset 0 0 0 1px rgba(0,0,0,0.15);
/* Use: Active/pressed states */
```

---

## 📱 Responsive Breakpoints 响应式断点

```
Small Mobile:   <479px   (Minimum layout)
Mobile:         479-640px (Single column)
Large Mobile:   640-767px (Wider content)
Tablet:         768-991px (2-column grids)
Desktop:        992px+   (Full layout)
```

### Typography Scaling
```
Desktop H1:  64px
Tablet H1:   36px
Mobile H1:   28px
```

---

## ✅ Do's and Don'ts 使用准则

### ✅ DO
- Use Parchment (#f5f4ed) as main background
- Keep all neutrals warm-toned
- Use Serif for all headings at weight 500
- Apply generous line-height (1.60) for body
- Use ring shadows for interactive states
- Alternate light/dark sections for rhythm
- Round corners generously (8-32px)

### ❌ DON'T
- Use cool blue-grays anywhere
- Use bold (700+) weight on serif headings
- Introduce saturated colors beyond Terracotta
- Use sharp corners (<6px) on UI elements
- Apply heavy drop shadows
- Use pure white as page background
- Reduce body line-height below 1.40

---

## 🔗 CSS Variables Quick Access

```css
/* Copy these for quick reference */
var(--parchment)           /* Main background */
var(--terracotta-brand)    /* Primary accent */
var(--anthropic-near-black) /* Primary text */
var(--olive-gray)          /* Secondary text */
var(--border-cream)        /* Light borders */
var(--ring-warm)           /* Interactive rings */
var(--font-serif)          /* Heading font */
var(--font-sans)           /* Body font */
var(--font-mono)           /* Code font */
```

---

## 💡 Pro Tips 专业技巧

1. **Reading Flow**: The 1.60 line-height creates a book-like reading experience. Trust it.

2. **Visual Hierarchy**: Let the serif/sans distinction do the work. Serif = important, Sans = functional.

3. **Warmth Consistency**: Every gray has yellow-brown undertones. This is intentional and crucial.

4. **Shadow Philosophy**: Ring shadows are borders pretending to be shadows. Subtle depth > dramatic lifts.

5. **Section Rhythm**: Alternate light/dark sections like chapters in a book. Creates natural pauses.

---

*Print this card and keep it handy while designing with the Claude Anthropic theme!* 📋✨

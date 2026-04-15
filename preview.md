# Claude Anthropic Theme Preview

这是 **Claude Anthropic** Typora 主题的完整预览文档。

---

## Typography 排版系统

### Headings 标题

# Heading 1 - Serif 64px, Weight 500

The largest heading with tight line-height (1.10), creating maximum impact like a book title.

## Heading 2 - Serif 52px, Weight 500

Section headings that anchor major content areas with authoritative presence.

### Heading 3 - Serif 36px, Weight 500

Sub-section markers with relaxed line-height for comfortable reading.

#### Heading 4 - Serif 32px, Weight 500

Card titles and feature names with tight spacing.

##### Heading 5 - Serif 25px, Weight 500

Smaller section titles maintaining serif hierarchy.

###### Heading 6 - Serif 20px, Weight 500

The smallest heading level, still carrying serif authority.

---

## Body Text 正文

This is standard body text at 16px with a generous 1.60 line-height. The warm parchment background (`#f5f4ed`) and near-black text (`#141413`) create a reading experience closer to a printed page than a digital screen.

**Bold text** stands out with 600 weight while *italic text* adds subtle emphasis in olive gray. You can also use ~~strikethrough~~ for deleted content or ==highlighted text== for important passages.

> This is a blockquote. It uses the Anthropic Serif font at 17px with a terracotta left border and ivory background. Perfect for emphasizing key insights, quotations, or important notes that deserve special attention in your document.

---

## Links 链接

Here's a [sample link](https://example.com) that demonstrates the link styling with a warm underline that transitions to terracotta on hover.

---

## Lists 列表

### Unordered List

- First item with comfortable spacing
- Second item maintaining 1.60 line-height
  - Nested item indented properly
  - Another nested point
- Third item in the main list

### Ordered List

**多级编号样式展示：**

1. 第一级 - 阿拉伯数字 (Arabic numerals)
   1. 第二级 - 罗马数字 (Roman numerals)
      1. 第三级 - 英文字母 (Letters)
      2. Third level item b
      3. Third level item c
   2. Second level item ii
   3. Second level item iii
2. First level item 2
   1. Nested under second item
      1. Deep nesting example a
      2. Deep nesting example b
3. First level item 3

**传统嵌套示例：**

1. First numbered item
2. Second numbered item
   i. Nested numbered item (Roman)
      a. Another nested point (Letter)
      b. Yet another point
   ii. Second nested item
3. Third numbered item

### Task List

- [x] Completed task with checked box
- [ ] Pending task awaiting action
- [ ] Another incomplete task
- [x] Final completed item

---

## Code 代码

### Inline Code

Use `inline code` for technical terms like `const variable` or `function_name()` within paragraphs. The code appears with a warm sand background and subtle border.

### Code Block

```javascript
// JavaScript example with syntax highlighting
function calculateTotal(items) {
  const taxRate = 0.08;
  const subtotal = items.reduce((sum, item) => sum + item.price, 0);
  const total = subtotal * (1 + taxRate);
  
  return {
    subtotal: subtotal.toFixed(2),
    tax: (subtotal * taxRate).toFixed(2),
    total: total.toFixed(2)
  };
}

const items = [
  { name: 'Book', price: 29.99 },
  { name: 'Pen', price: 4.99 }
];

console.log(calculateTotal(items));
```

```
# Python example demonstrating clean code presentation
class DocumentTheme:
    def __init__(self, name, palette):
        self.name = name
        self.palette = palette
        self.font_family = {
            'heading': 'Serif',
            'body': 'Sans',
            'code': 'Mono'
        }
    
    def apply_theme(self, document):
        """Apply the theme to a document."""
        for element in document.elements:
            element.style = self.get_style(element.type)
        return document
    
    def get_style(self, element_type):
        styles = {
            'h1': {'size': '64px', 'weight': 500},
            'body': {'size': '16px', 'line_height': 1.60}
        }
        return styles.get(element_type, {})

# Create and apply theme
claude_theme = DocumentTheme(
    'Claude Anthropic',
    {'background': '#f5f4ed', 'accent': '#c96442'}
)
```

```
/* CSS example showing theme variables */
:root {
  --parchment: #f5f4ed;
  --terracotta: #c96442;
  --near-black: #141413;
  
  font-family: system-ui, sans-serif;
  line-height: 1.60;
}

body {
  background-color: var(--parchment);
  color: var(--near-black);
}
```

---

## Tables 表格

### Feature Comparison

| Feature | Description | Status | Priority |
|---------|-------------|--------|----------|
| Warm Palette | Exclusively warm-toned neutrals | ✅ Complete | High |
| Serif Headings | Magazine-style typography | ✅ Complete | High |
| Ring Shadows | Border-like depth without borders | ✅ Complete | Medium |
| Responsive | Adapts to all screen sizes | ✅ Complete | High |
| Dark Mode | System-level dark theme support | ✅ Complete | Medium |
| Custom Fonts | Anthropic type family | ⏳ Planned | Low |

### Pricing Example

| Plan | Price | Features | Best For |
|------|-------|----------|----------|
| Basic | $0 | Core features, limited exports | Personal use |
| Pro | $12/mo | Unlimited exports, themes | Professionals |
| Team | $49/mo | Collaboration, admin controls | Teams |

---

## Images 图片

![Sample Image](https://th.wallhaven.cc/lg/5y/5ykjy8.jpg)

*Image caption appears below in stone gray italic text*

---

## Horizontal Rule 分隔线

Content above the rule.

---

Content below the rule, clearly separated with a warm cream border.

---

## Mathematical Equations 数学公式

Inline math: $E = mc^2$

Display math:

$$
\int_{a}^{b} f(x) \, dx = F(b) - F(a)
$$

$$
\frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$

---

## Footnotes 脚注

Here's some text with a footnote reference.[^1] And another one.[^2]

[^1]: This is the first footnote. It appears at the bottom of the document in smaller, olive gray text.

[^2]: The second footnote demonstrates how multiple footnotes are organized and styled.

---

## Special Elements 特殊元素

### Mark/Highlight

This text is <mark>highlighted</mark> using the mark element with a warm sand background.

### Superscript and Subscript

H<sub>2</sub>O is water, and E=mc<sup>2</sup> is Einstein's equation.

---

## Table of Contents 目录

The theme styles the auto-generated table of contents with an ivory background and comfortable border radius.

---

## Front Matter YAML

```
---
title: Claude Anthropic Theme
author: Your Name
date: 2026-04-15
tags:
  - typora
  - theme
  - design
---
```

---

## Color Palette Reference 色彩参考

### Primary Colors

<div style="display: flex; gap: 16px; flex-wrap: wrap; margin: 24px 0;">
  <div style="background: #141413; color: #faf9f5; padding: 16px; border-radius: 8px; min-width: 120px;">
    <strong>Near Black</strong><br>#141413
  </div>
  <div style="background: #c96442; color: #faf9f5; padding: 16px; border-radius: 8px; min-width: 120px;">
    <strong>Terracotta</strong><br>#c96442
  </div>
  <div style="background: #d97757; color: #faf9f5; padding: 16px; border-radius: 8px; min-width: 120px;">
    <strong>Coral</strong><br>#d97757
  </div>
</div>

### Surface Colors

<div style="display: flex; gap: 16px; flex-wrap: wrap; margin: 24px 0;">
  <div style="background: #f5f4ed; color: #141413; padding: 16px; border-radius: 8px; min-width: 120px; border: 1px solid #e8e6dc;">
    <strong>Parchment</strong><br>#f5f4ed
  </div>
  <div style="background: #faf9f5; color: #141413; padding: 16px; border-radius: 8px; min-width: 120px; border: 1px solid #e8e6dc;">
    <strong>Ivory</strong><br>#faf9f5
  </div>
  <div style="background: #e8e6dc; color: #4d4c48; padding: 16px; border-radius: 8px; min-width: 120px;">
    <strong>Warm Sand</strong><br>#e8e6dc
  </div>
  <div style="background: #30302e; color: #faf9f5; padding: 16px; border-radius: 8px; min-width: 120px;">
    <strong>Dark Surface</strong><br>#30302e
  </div>
</div>

### Neutral Grays

<div style="display: flex; gap: 16px; flex-wrap: wrap; margin: 24px 0;">
  <div style="background: #4d4c48; color: #faf9f5; padding: 16px; border-radius: 8px; min-width: 100px;">
    <strong>Charcoal</strong><br>#4d4c48
  </div>
  <div style="background: #5e5d59; color: #faf9f5; padding: 16px; border-radius: 8px; min-width: 100px;">
    <strong>Olive Gray</strong><br>#5e5d59
  </div>
  <div style="background: #87867f; color: #faf9f5; padding: 16px; border-radius: 8px; min-width: 100px;">
    <strong>Stone</strong><br>#87867f
  </div>
  <div style="background: #b0aea5; color: #141413; padding: 16px; border-radius: 8px; min-width: 100px;">
    <strong>Silver</strong><br>#b0aea5
  </div>
</div>

---

## Writing Sample 写作示例

### The Art of Thoughtful Design

In a world saturated with cold, futuristic interfaces, there's something profoundly comforting about warmth. The Claude design system embraces this truth, choosing parchment over pixel-perfect whites, terracotta over electric blues, and serif typography over sterile sans-serifs.

> Design is not just what it looks like and feels like. Design is how it works. — Steve Jobs

The choice of a warm neutral palette isn't merely aesthetic—it's psychological. Every gray carries a yellow-brown undertone, creating a space that feels *lived-in* rather than sterile. When you read text set against `#f5f4ed`, your eyes don't strain against the harsh contrast of pure white. Instead, they relax into the gentle warmth, much like reading a well-loved book.

#### Typography as Voice

The decision to use a single weight (500) for all serif headings creates a consistent "voice" throughout the document. Whether it's a massive H1 at 64px or a modest H6 at 20px, the medium weight says: *"I'm confident but not shouting. I'm authoritative but approachable."*

Body text flows at 1.60 line-height—generous by web standards, but natural for extended reading. This isn't a dashboard to scan; it's a document to *read*.

```
The best designs are invisible. They don't call attention to themselves;
they simply make the content shine. Like good editing, good design
knows when to step back and let the words speak.
```

#### The Power of Restraint

Notice what's absent: no gradients, no drop shadows, no neon accents. The design achieves depth through subtle ring shadows (`0px 0px 0px 1px`) and the strategic alternation between light and dark sections. This restraint creates sophistication.

**Key takeaway**: Warmth doesn't mean clutter. The Claude system proves that a restrained, warm palette can be more inviting than a rainbow of cool colors.

---

## Conclusion

This preview demonstrates the complete Claude Anthropic theme for Typora. Every element—from headings to code blocks, from tables to blockquotes—has been carefully crafted to create a warm, editorial reading experience.

Enjoy writing in comfort! ✍️

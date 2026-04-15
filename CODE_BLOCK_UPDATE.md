# 代码块样式更新说明

## 📝 更新内容

**更新日期：** 2026-04-15  
**版本：** v1.0.1 (patch)

---

## 🎨 变更详情

### 之前（深色背景）
```css
pre {
  background-color: var(--dark-surface);  /* #30302e - 深色 */
  color: var(--warm-silver);              /* #b0aea5 - 暖银色 */
  border: 1px solid var(--border-dark);   /* #30302e - 深色边框 */
}
```

### 之后（浅色背景）✅
```css
pre {
  background-color: var(--ivory);         /* #faf9f5 - 象牙白 */
  color: var(--charcoal-warm);            /* #4d4c48 - 炭灰色 */
  border: 1px solid var(--border-cream);  /* #f0eee6 - 奶油色边框 */
}
```

---

## 🎯 设计理念

### 为什么改为浅色？

1. **统一的温暖基调**
   - 保持整个主题的浅色调一致性
   - 避免深色代码块在羊皮纸背景上显得突兀
   - 更符合"纸质阅读"的视觉体验

2. **更好的可读性**
   - 浅色背景减少眼部疲劳
   - 炭灰色文字在象牙白背景上清晰易读
   - 适合长时间阅读和编辑代码

3. **设计哲学一致**
   - Claude 设计系统强调温暖和亲切
   - 浅色代码块更符合"文学沙龙"的氛围
   - 与引用块、卡片等元素保持视觉统一

---

## 📊 色彩对比

| 元素 | 之前（深色） | 之后（浅色） |
|------|------------|------------|
| 背景色 | #30302e (Dark Surface) | #faf9f5 (Ivory) |
| 文字色 | #b0aea5 (Warm Silver) | #4d4c48 (Charcoal Warm) |
| 边框色 | #30302e (Border Dark) | #f0eee6 (Border Cream) |
| 对比度 | 中等 | 良好 |

---

## 🌙 暗色模式

暗色模式下，代码块会自动适配为深色背景，通过 CSS 变量系统实现：

```css
@media (prefers-color-scheme: dark) {
  :root {
    --ivory: var(--dark-surface);      /* 自动变为深色 */
    --charcoal-warm: var(--warm-silver); /* 文字变为亮色 */
    --border-cream: var(--border-dark);  /* 边框变为深色 */
  }
}
```

**结果：**
- ✅ 浅色模式：象牙白背景 + 炭灰文字
- ✅ 暗色模式：深色背景 + 暖银文字
- ✅ 自动切换，无需手动调整

---

## 🔄 影响的文件

### 已更新
1. ✅ `claude-anthropic.css` - 核心样式文件
2. ✅ `README.md` - 主题介绍文档
3. ✅ `QUICK_REFERENCE.md` - 快速参考卡片

### 无需更新
- `preview.md` - 预览文档中的代码示例会自动应用新样式
- 其他文档文件 - 不涉及代码块样式描述

---

## 💡 使用建议

### 如果您喜欢深色代码块

可以通过自定义 CSS 恢复深色风格：

```css
/* 在 claude-anthropic.css 的 :root 后添加 */
pre {
  background-color: #30302e !important;
  color: #b0aea5 !important;
  border-color: #30302e !important;
}
```

或者创建自定义变量覆盖：

```css
:root {
  --code-bg: #30302e;
  --code-text: #b0aea5;
  --code-border: #30302e;
}

pre {
  background-color: var(--code-bg);
  color: var(--code-text);
  border-color: var(--code-border);
}
```

---

## ✅ 测试清单

安装更新后，请检查：

- [ ] 代码块背景是浅色（象牙白 #faf9f5）
- [ ] 代码文字是炭灰色（#4d4c48）
- [ ] 代码块边框是奶油色（#f0eee6）
- [ ] 行内代码仍然是暖沙色背景
- [ ] 暗色模式下代码块自动变为深色
- [ ] 代码可读性良好

---

## 📸 视觉效果对比

### 浅色模式（更新后）
```
┌─────────────────────────────────┐
│  background: #faf9f5 (象牙白)    │
│  color: #4d4c48 (炭灰)          │
│  border: #f0eee6 (奶油)         │
│                                 │
│  def hello():                   │
│      print("Hello!")            │
└─────────────────────────────────┘
```

### 暗色模式（自动适配）
```
┌─────────────────────────────────┐
│  background: #30302e (深色)      │
│  color: #b0aea5 (暖银)          │
│  border: #30302e (深色)         │
│                                 │
│  def hello():                   │
│      print("Hello!")            │
└─────────────────────────────────┘
```

---

## 🎉 总结

这次更新将代码块从深色背景改为浅色背景，更好地融入了 Claude Anthropic 主题的温暖、 editorial 设计风格。

**核心优势：**
- ✅ 视觉一致性更强
- ✅ 阅读体验更舒适
- ✅ 符合设计哲学
- ✅ 暗色模式自动适配

**享受更加温暖的代码编写体验！** ✍️💻

# Claude Anthropic Dark - 快速参考

## 🎨 核心色彩

### 背景色
```css
页面背景:    #141413  /* Deep Dark - 温暖近黑 */
卡片/容器:   #30302e  /* Dark Surface - 深炭色 */
交互表面:    #3d3d3a  /* Dark Warm - 深暖色 */
```

### 文本色
```css
标题:        #faf9f5  /* Ivory - 象牙白 */
主要正文:    #b0aea5  /* Warm Silver - 暖银色 */
次要文本:    #b0aea5  /* Warm Silver - 暖银色 */
元数据:      #87867f  /* Stone Gray - 石灰色 */
链接:        #d97757  /* Coral Accent - 珊瑚色 */
```

### 强调色
```css
品牌主色:    #c96442  /* Terracotta - 赤陶 */
链接悬停:    #c96442  /* Terracotta - 赤陶 */
错误状态:    #b53333  /* Error Crimson - 深红 */
焦点环:      #3898ec  /* Focus Blue - 焦点蓝 */
```

### 边框色
```css
标准边框:    #30302e  /* Border Dark */
突出边框:    #3d3d3a  /* Border Warm */
环状阴影:    #5e5d59  /* Ring Warm */
```

## 📝 排版规范

### 字体族
```css
标题:        "Anthropic Serif", Georgia, serif
正文:        "Anthropic Sans", Arial, system-ui, sans-serif
代码:        "Anthropic Mono", "SF Mono", Monaco, monospace
```

### 字号层次
| 元素 | 字号 | 字重 | 行高 |
|------|------|------|------|
| H1 | 64px | 500 | 1.10 |
| H2 | 52px | 500 | 1.20 |
| H3 | 36px | 500 | 1.30 |
| H4 | 32px | 500 | 1.10 |
| H5 | 25px | 500 | 1.20 |
| H6 | 20px | 500 | 1.20 |
| 正文 | 16px | 400 | 1.60 |
| 引言 | 17px | 400 | 1.60 |
| 代码 | 15px | 400 | 1.60 |
| 小字 | 14px | 400 | 1.43 |

## 🎯 组件样式速查

### 代码块
```css
背景:        #30302e  /* Dark Surface */
文字:        #b0aea5  /* Warm Silver */
边框:        #30302e  /* Border Dark */
圆角:        16px     /* Very Rounded */
内边距:      24px
```

### 引用块
```css
背景:        #30302e  /* Dark Surface */
文字:        #b0aea5  /* Warm Silver */
左边框:      4px solid #c96442
字体:        Serif
圆角:        8px (右侧)
```

### 表格
```css
表头背景:    #3d3d3a  /* Dark Warm */
单元格背景:  #30302e  /* Dark Surface */
表头文字:    #b0aea5  /* Warm Silver */
单元格文字:  #faf9f5  /* Ivory */
边框:        #30302e  /* Border Dark */
悬停背景:    #30302e  /* Dark Surface */
```

### 列表
```css
有序列表层级:
  Level 1:   1, 2, 3          (阿拉伯数字)
  Level 2:   i, ii, iii       (罗马数字)
  Level 3:   a, b, c          (小写字母)
  Level 4+:  1, 2, 3          (重置)

任务复选框:  accent-color: #c96442
```

### 链接
```css
默认:        #d97757 + 下划线
悬停:        #c96442 + 深色下划线
脚注链接:    #c96442 (无下划线)
```

## 📏 间距系统

基于 8px 基础单位：

```css
--space-xs:    3px
--space-sm:    4px
--space-md:    6px
--space-base:  8px
--space-lg:    10px
--space-xl:    12px
--space-2xl:   16px
--space-3xl:   20px
--space-4xl:   24px
--space-5xl:   30px
```

常用组合：
- 段落间距: `margin-bottom: 16px` (--space-2xl)
- 章节间距: `margin-top: 30px` (--space-5xl)
- 代码块间距: `margin: 20px 0` (--space-3xl)
- 列表项间距: `margin-bottom: 8px` (--space-base)

## 🔲 圆角系统

```css
--radius-sharp:       4px   /* 锐利 */
--radius-subtle:      6px   /* 微妙 */
--radius-comfortable: 8px   /* 舒适 - 按钮、卡片 */
--radius-generous:    12px  /* 慷慨 - 主按钮、输入框 */
--radius-very:        16px  /* 非常 - 代码块、视频 */
--radius-highly:      24px  /* 高度 - 标签 */
--radius-maximum:     32px  /* 最大 - Hero、大卡片 */
```

## 🌟 设计原则

### ✅ Do's
- 使用温暖的深色调 (#141413, #30302e)
- 保持 exclusively 暖色调中性色
- Serif 标题使用 500 字重
- generous 行高 (1.60)
- 环状阴影而非传统投影
- generous 圆角 (8-32px)

### ❌ Don'ts
- 不使用冷蓝灰色
- 不使用纯黑 (#000000) 或纯白 (#ffffff)
- 不引入饱和色彩（除 Terracotta）
- 不使用锐利边角 (< 6px)
- 不使用重型投影
- 不降低正文字体行高至 1.40 以下

## 📱 响应式断点

```css
Small Mobile:  <479px   /* 最小布局 */
Mobile:        479-640px /* 单列 */
Large Mobile:  640-767px /* 稍宽 */
Tablet:        768-991px /* 2列网格 */
Desktop:       992px+    /* 完整布局 */
```

移动端调整：
- H1: 64px → 28px
- H2: 52px → 25px
- H3: 36px → 20px
- 内边距减少 50%

## 🔧 CSS 变量自定义

```css
:root {
  /* 背景深度 */
  --parchment: #141413;  /* 页面背景 */
  --ivory: #30302e;      /* 卡片表面 */
  
  /* 文本亮度 */
  --charcoal-warm: #b0aea5;  /* 主要文本 */
  --olive-gray: #b0aea5;     /* 次要文本 */
  
  /* 强调色 */
  --terracotta-brand: #c96442;  /* 品牌色 */
  --coral-accent: #d97757;      /* 珊瑚强调 */
  
  /* 边框 */
  --border-cream: #30302e;  /* 标准边框 */
  --border-warm: #3d3d3a;   /* 突出边框 */
}
```

## 💡 使用场景

### 最佳使用时机
- 🌙 夜间工作（20:00 - 06:00）
- 🕯️ 昏暗环境（低光照条件）
- 👁️ 眼部敏感（减少蓝光）
- 🎯 深度专注（减少干扰）
- ⏰ 长时间写作（减少疲劳）

### 切换到浅色版本的时机
- ☀️ 白天明亮环境
- 💡 强光办公室
- 📄 需要打印预览
- 🎨 设计审查（更接近最终输出）

## 🚀 快速安装

```bash
# 1. 复制文件到 Typora 主题文件夹
cp claude-anthropic-dark.css ~/Library/Application\ Support/abnerworks/Typora/themes/  # macOS
# 或
cp claude-anthropic-dark.css %APPDATA%\Typora\themes\  # Windows

# 2. 重启 Typora

# 3. 在偏好设置中选择 "Claude Anthropic Dark"
```

## 📊 与浅色版对比

| 特性 | 浅色版 | 暗色版 |
|------|--------|--------|
| 背景 | #f5f4ed | #141413 |
| 卡片 | #faf9f5 | #30302e |
| 标题 | #141413 | #faf9f5 |
| 正文 | #141413 | #b0aea5 |
| 代码背景 | #faf9f5 | #30302e |
| 适用时间 | 日间 | 夜间 |

## 📚 相关文档

- [完整说明](README-DARK.md) - 详细设计规范
- [主题对比](THEME_COMPARISON.md) - 浅色 vs 暗色
- [安装指南](INSTALL-DARK.md) - 逐步安装说明
- [主 README](README.md) - 项目总览

---

**快速访问 • 温暖深夜 • 舒适阅读** 🌙✨

*提示：将此文件加入书签，方便快速查阅色彩和样式规范。*

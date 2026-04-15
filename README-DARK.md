# Claude Anthropic Dark Theme for Typora

## 概述

Claude Anthropic Dark 是专为 Typora 设计的暗色主题，基于 Claude (Anthropic) 的设计系统。它采用温暖的深色调，营造出舒适、富有编辑感的夜间阅读体验。

## 设计特色

### 🌙 温暖的暗色调
- **页面背景**: Deep Dark (#141413) - 温暖的近黑色，带有微妙的橄榄色调
- **卡片表面**: Dark Surface (#30302e) - 温暖的深炭色，用于容器和卡片
- **文本颜色**: Ivory (#faf9f5) 和 Warm Silver (#b0aea5) - 保持温暖的中性色调

### ✨ 核心特征
- ** exclusively 暖色调**: 所有中性色都带有黄棕底色，避免冷蓝灰色
- **环状阴影系统**: 使用 `0px 0px 0px 1px` 的温暖色调环状阴影
- **杂志级排版**: Serif 标题（Georgia）与 Sans-serif 正文（Arial）的经典组合
- **Terracotta 强调色**: 温暖的赤陶色 (#c96442) 作为主要品牌色

### 🎨 色彩系统

#### 主要颜色
- **Deep Dark** (`#141413`): 页面背景 - 最温暖的"黑色"
- **Dark Surface** (`#30302e`): 卡片和容器表面
- **Ivory** (`#faf9f5`): 主要文本颜色
- **Warm Silver** (`#b0aea5`): 次要文本和元数据

#### 强调色
- **Terracotta Brand** (`#c96442`): 主要 CTA 和品牌元素
- **Coral Accent** (`#d97757`): 链接和次要强调
- **Error Crimson** (`#b53333`): 错误状态

#### 边框和交互
- **Border Cream** (`#30302e`): 标准边框
- **Border Warm** (`#3d3d3a`): 突出边框
- **Ring Warm** (`#5e5d59`): 悬停/聚焦状态的环状阴影

### 📝 排版层次

| 元素 | 字体 | 大小 | 字重 | 行高 |
|------|------|------|------|------|
| H1 | Anthropic Serif | 64px | 500 | 1.10 |
| H2 | Anthropic Serif | 52px | 500 | 1.20 |
| H3 | Anthropic Serif | 36px | 500 | 1.30 |
| H4 | Anthropic Serif | 32px | 500 | 1.10 |
| H5 | Anthropic Serif | 25px | 500 | 1.20 |
| H6 | Anthropic Serif | 20px | 500 | 1.20 |
| 正文 | Anthropic Sans | 16px | 400 | 1.60 |
| 引言 | Anthropic Serif | 17px | 400 | 1.60 |
| 代码 | Anthropic Mono | 15px | 400 | 1.60 |

### 🎯 组件样式

#### 代码块
- 背景: Dark Surface (#30302e)
- 文字: Warm Silver (#b0aea5)
- 边框: Border Cream (#30302e)
- 圆角: 16px (非常圆润)

#### 引用块
- 背景: Dark Surface (#30302e)
- 左边框: 4px solid Terracotta (#c96442)
- 文字: Warm Silver (#b0aea5)
- 字体: Anthropic Serif

#### 表格
- 表头背景: Dark Warm (#3d3d3a)
- 单元格背景: Dark Surface (#30302e)
- 悬停效果: 更深的深色背景
- 边框: 温暖的奶油色

#### 列表
- 有序列表层级:
  - Level 1: 阿拉伯数字 (1, 2, 3)
  - Level 2: 小写罗马数字 (i, ii, iii)
  - Level 3: 小写字母 (a, b, c)
  - Level 4+: 重置为阿拉伯数字

## 安装方法

### 方法一：手动安装

1. 下载 `claude-anthropic-dark.css` 文件
2. 打开 Typora，进入 **偏好设置** → **外观** → **打开主题文件夹**
3. 将 CSS 文件复制到该文件夹
4. 重启 Typora
5. 在 **偏好设置** → **外观** → **主题** 中选择 "Claude Anthropic Dark"

### 方法二：使用 package.json

1. 确保 `package-dark.json` 重命名为 `package.json`
2. 将整个文件夹复制到 Typora 主题目录
3. 重启 Typora 并选择主题

## 与浅色版本的对比

| 特性 | 浅色版本 | 暗色版本 |
|------|---------|---------|
| 页面背景 | Parchment (#f5f4ed) | Deep Dark (#141413) |
| 卡片表面 | Ivory (#faf9f5) | Dark Surface (#30302e) |
| 主要文本 | Near Black (#141413) | Ivory (#faf9f5) |
| 次要文本 | Olive Gray (#5e5d59) | Warm Silver (#b0aea5) |
| 代码块背景 | Ivory (#faf9f5) | Dark Surface (#30302e) |
| 边框颜色 | Border Cream (#f0eee6) | Border Dark (#30302e) |
| 适用场景 | 日间阅读 | 夜间阅读 |

## 设计原则

### ✅ 应该做的
- 使用 Deep Dark (#141413) 作为主要背景
- 保持所有中性色的温暖色调
- 使用环状阴影而非传统投影
- Serif 标题保持 500 字重
-  generous 行高 (1.60) 营造文学阅读体验
- 交替使用明暗区域创造章节感

### ❌ 不应该做的
- 不要使用冷蓝灰色
- 不要使用纯黑 (#000000) 或纯白 (#ffffff)
- 不要引入饱和色彩
- 不要使用锐利边角 (< 6px)
- 不要使用重型投影
- 不要降低正文字体行高至 1.40 以下

## 响应式设计

主题针对不同屏幕尺寸进行了优化：

- **桌面端** (>992px): 完整多列布局，最大 64px 标题
- **平板端** (768-991px): 2 列网格，压缩导航
- **移动端** (<768px): 单列布局，缩小的标题尺寸
- **小屏手机** (<480px): 最小布局，紧凑排版

## 版权说明

本主题基于 Anthropic 设计系统创建，仅供个人使用。原始设计版权归 Anthropic 所有。

## 更新日志

### v1.0.0 (2026-04-15)
- 初始发布
- 完整的暗色主题实现
- 基于 Claude Design System 规范
- 支持所有 Typora Markdown 元素
- 响应式设计适配

## 技术支持

如有问题或建议，请访问：
- GitHub Issues: https://github.com/yourusername/typora-theme-claude-anthropic/issues

---

**享受温暖的夜间阅读体验！** 🌙✨

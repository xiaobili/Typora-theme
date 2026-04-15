# 🚀 快速开始 - Claude Anthropic Dark Theme

## ⚡ 30 秒快速安装

### 步骤 1: 找到主题文件夹

**macOS:**
```bash
open ~/Library/Application\ Support/abnerworks/Typora/themes/
```

**Windows:**
```bash
explorer %APPDATA%\Typora\themes\
```

**Linux:**
```bash
xdg-open ~/.config/Typora/themes/
```

或者在 Typora 中：
- **偏好设置** → **外观** → **打开主题文件夹**

### 步骤 2: 复制主题文件

将 `claude-anthropic-dark.css` 复制到打开的主题文件夹

### 步骤 3: 启用主题

1. 重启 Typora
2. **偏好设置** → **外观** → **主题**
3. 选择 **"Claude Anthropic Dark"**
4. ✅ 完成！

---

## 📋 完整文件清单

### 必需文件（至少需要一个）

#### ☀️ 浅色版本
- ✅ `claude-anthropic.css` - 浅色主题文件
- 📄 `package.json` - 浅色版本配置（可选）

#### 🌙 暗色版本
- ✅ `claude-anthropic-dark.css` - 暗色主题文件
- 📄 `package-dark.json` - 暗色版本配置（可选）

### 推荐文档

#### 📖 入门必读
- [README.md](README.md) - 项目总览和双主题介绍
- [INSTALL.md](INSTALL.md) - 浅色版本安装指南
- [INSTALL-DARK.md](INSTALL-DARK.md) - 暗色版本安装指南

#### 🎨 深入了解
- [README-DARK.md](README-DARK.md) - 暗色主题详细说明
- [THEME_COMPARISON.md](THEME_COMPARISON.md) - 浅色 vs 暗色对比
- [Design System Inspired by Claude (Anthropic).md](Design%20System%20Inspired%20by%20Claude%20(Anthropic).md) - 设计规范原文

#### ⚡ 快速参考
- [QUICK_REFERENCE.md](QUICK_REFERENCE.md) - 浅色版快速参考
- [QUICK_REFERENCE-DARK.md](QUICK_REFERENCE-DARK.md) - 暗色版快速参考
- [QUICK_START.md](QUICK_START.md) - 快速开始指南

#### 📚 其他资源
- [CHANGELOG.md](CHANGELOG.md) - 版本历史
- [PROJECT_STRUCTURE.md](PROJECT_STRUCTURE.md) - 项目结构说明
- [RELEASE_SUMMARY-DARK.md](RELEASE_SUMMARY-DARK.md) - 暗色版本发布总结
- [LIST_STYLES.md](LIST_STYLES.md) - 列表样式说明
- [CODE_BLOCK_UPDATE.md](CODE_BLOCK_UPDATE.md) - 代码块样式说明
- [SUMMARY.md](SUMMARY.md) - 项目总结
- [preview.md](preview.md) - 主题预览测试文件

---

## 🎯 选择指南

### 我应该使用哪个版本？

#### 选择浅色版本，如果：
- ☀️ 主要在白天使用 Typora
- 💡 工作环境光线充足
- 📖 喜欢纸质书的阅读感觉
- 📄 经常需要打印文档
- ✍️ 进行创意写作或日常记录

#### 选择暗色版本，如果：
- 🌙 经常在夜间或昏暗环境工作
- 👁️ 眼睛对亮光敏感
- 🎯 需要长时间深度专注
- 💻 主要进行编码或技术写作
- 😌 希望减少眼部疲劳

#### 同时安装两个版本，如果：
- 🔄 想根据时间自动切换
- 📊 不同项目使用不同主题
- 🎨 想对比效果后决定
- 👥 团队中有不同偏好的成员

---

## 🔧 高级安装选项

### 选项 1: 仅安装暗色版本

```bash
# macOS
cp claude-anthropic-dark.css ~/Library/Application\ Support/abnerworks/Typora/themes/

# Windows
copy claude-anthropic-dark.css %APPDATA%\Typora\themes\

# Linux
cp claude-anthropic-dark.css ~/.config/Typora/themes/
```

### 选项 2: 同时安装两个版本

```bash
# macOS
cp claude-anthropic.css ~/Library/Application\ Support/abnerworks/Typora/themes/
cp claude-anthropic-dark.css ~/Library/Application\ Support/abnerworks/Typora/themes/

# Windows
copy claude-anthropic.css %APPDATA%\Typora\themes\
copy claude-anthropic-dark.css %APPDATA%\Typora\themes\

# Linux
cp claude-anthropic.css ~/.config/Typora/themes/
cp claude-anthropic-dark.css ~/.config/Typora/themes/
```

### 选项 3: 完整安装（包含所有文档）

```bash
# 克隆整个仓库
git clone https://github.com/yourusername/typora-theme-claude-anthropic.git

# 仅复制主题文件到 Typora
cp typora-theme-claude-anthropic/claude-anthropic*.css ~/Library/Application\ Support/abnerworks/Typora/themes/
```

---

## ✅ 验证安装

安装成功后，您应该看到：

### 视觉检查清单

- [ ] Typora 背景变为深暖色调 (#141413)
- [ ] 标题使用衬线字体，颜色为象牙白 (#faf9f5)
- [ ] 正文使用无衬线字体，颜色为暖银色 (#b0aea5)
- [ ] 代码块背景为深炭色 (#30302e)
- [ ] 引用块左侧有赤陶色边框 (#c96442)
- [ ] 链接显示为珊瑚色 (#d97757)
- [ ] 表格有深色表头和悬停效果
- [ ] 滚动条为温暖深色调

### 功能检查清单

- [ ] 可以正常创建和编辑 Markdown 文档
- [ ] 所有标题层级显示正确
- [ ] 代码块语法高亮正常
- [ ] 表格渲染正确
- [ ] 图片显示正常
- [ ] 列表编号系统工作（1, i, a）
- [ ] 引用块样式正确
- [ ] 侧边栏主题适配

---

## 🎨 自定义主题

### 快速自定义（修改 CSS 变量）

编辑 `claude-anthropic-dark.css` 文件的 `:root` 部分：

```css
:root {
  /* 调整背景深度 */
  --parchment: #141413;  /* 更暗: #0a0a09, 更亮: #1e1e1d */
  
  /* 调整卡片表面 */
  --ivory: #30302e;      /* 更暗: #252524, 更亮: #3b3b39 */
  
  /* 调整文本亮度 */
  --charcoal-warm: #b0aea5;  /* 更亮: #c0beb5, 更暗: #a09e95 */
  
  /* 调整强调色 */
  --terracotta-brand: #c96442;  /* 保持温暖赤陶色 */
}
```

### 创建自定义变体

1. 复制 `claude-anthropic-dark.css` 为新文件
2. 重命名为 `my-custom-dark.css`
3. 修改 CSS 变量
4. 更新文件顶部的主题名称注释
5. 重启 Typora 并选择新主题

---

## 🔄 主题切换技巧

### 方法 1: 手动切换（推荐）

```
Typora 偏好设置 → 外观 → 主题 → 选择想要的版本
```

**优点**: 
- ✅ 完全控制
- ✅ 即时生效
- ✅ 无需额外工具

**缺点**:
- ❌ 需要手动操作

### 方法 2: 键盘快捷键（需配置）

macOS 可以使用 Automator 或 AppleScript 创建快捷切换脚本。

### 方法 3: 系统级自动切换

某些第三方工具可以根据时间或光照条件自动切换 Typora 主题。

---

## ❓ 常见问题

### Q1: 主题列表中没有 "Claude Anthropic Dark"？

**A**: 
1. 确认文件名完全正确：`claude-anthropic-dark.css`
2. 确认文件在正确的主题文件夹
3. 完全关闭并重启 Typora
4. 检查文件权限

### Q2: 如何卸载主题？

**A**: 
1. 关闭 Typora
2. 从主题文件夹删除对应的 CSS 文件
3. 重启 Typora
4. 选择其他主题

### Q3: 可以同时激活两个主题吗？

**A**: 不可以，Typora 一次只能激活一个主题。但可以快速切换。

### Q4: 暗色版本会影响导出的 PDF 吗？

**A**: 是的，导出的 PDF 会反映当前激活的主题样式。

### Q5: 可以在其他 Markdown 编辑器中使用吗？

**A**: 可能可以，但需要针对该编辑器调整 CSS 选择器。

---

## 📚 下一步

### 新手路径
1. ✅ 安装主题
2. 📖 阅读 [README.md](README.md) 了解特色
3. 🎨 查看 [preview.md](preview.md) 测试效果
4. ⚡ 收藏 [QUICK_REFERENCE-DARK.md](QUICK_REFERENCE-DARK.md) 作为速查
5. ✍️ 开始写作！

### 进阶路径
1. 📚 阅读 [README-DARK.md](README-DARK.md) 了解设计规范
2. 🔍 研究 [THEME_COMPARISON.md](THEME_COMPARISON.md) 理解差异
3. 🔧 尝试自定义 CSS 变量
4. 🎨 创建自己的变体
5. 💡 分享你的定制给社区

### 专家路径
1. 📖 研读 [Design System Inspired by Claude (Anthropic).md](Design%20System%20Inspired%20by%20Claude%20(Anthropic).md)
2. 🔬 分析 CSS 源码结构
3. 🛠️ 贡献代码改进主题
4. 📝 撰写教程帮助他人
5. 🌟 成为主题维护者

---

## 🆘 获取帮助

### 文档资源
- 📖 完整文档: 查看所有 `.md` 文件
- 🔍 搜索: 使用 GitHub 搜索功能
- 📋 Issues: 查看已解决的问题

### 社区支持
- 💬 GitHub Issues: 提问和讨论
- 🐛 Bug 报告: 详细描述 + 截图
- 💡 功能建议: 说明使用场景
- 🎨 展示作品: 分享你的自定义版本

### 直接联系
- 📧 Email: （如果有）
- 🐦 Twitter: （如果有）
- 💼 LinkedIn: （如果有）

---

## 🎉 开始写作！

安装完成，现在您可以：

1. 📝 创建新的 Markdown 文档
2. 🌙 享受温暖的夜间写作体验
3. ✨ 感受 Claude 设计系统的优雅
4. 🎨 根据需要切换浅色/暗色版本
5. 💪 提高写作效率和舒适度

**祝您写作愉快！** ✍️🌙✨

---

*提示：将此页面加入书签，方便日后快速参考。*

**最后更新**: 2026-04-15  
**版本**: v1.0.0 (Dark)  
**维护者**: Claude Anthropic Theme Team

# 安装指南 - Claude Anthropic Dark Theme

## 🌙 安装暗色主题

本文档详细说明如何安装 Claude Anthropic 暗色版本的 Typora 主题。

## 📋 前置要求

- ✅ Typora 编辑器（最新版本推荐）
- ✅ 操作系统支持暗色模式（可选，用于自动切换）
- ✅ 基本的文件操作能力

## 🚀 快速安装（3 步完成）

### 步骤 1：获取主题文件

确保您有以下文件：
- `claude-anthropic-dark.css` - 主题核心文件
- `package-dark.json` - 主题配置文件（可选）

### 步骤 2：打开 Typora 主题文件夹

**macOS:**
1. 打开 Typora
2. 点击菜单栏 **Typora** → **偏好设置** (或按 `Cmd + ,`)
3. 选择 **外观** 标签
4. 点击 **打开主题文件夹** 按钮

**Windows:**
1. 打开 Typora
2. 点击菜单栏 **文件** → **偏好设置** (或按 `Ctrl + ,`)
3. 选择 **外观** 标签
4. 点击 **打开主题文件夹** 按钮

**Linux:**
1. 打开 Typora
2. 点击菜单栏 **文件** → **偏好设置**
3. 选择 **外观** 标签
4. 点击 **打开主题文件夹** 按钮

### 步骤 3：复制主题文件

1. 将 `claude-anthropic-dark.css` 文件复制到打开的主题文件夹
2. （可选）如果需要完整的主题包信息，也可以复制其他相关文件
3. 关闭并重启 Typora

### 步骤 4：启用主题

1. 重新打开 Typora
2. 进入 **偏好设置** → **外观** → **主题**
3. 在下拉列表中选择 **"Claude Anthropic Dark"**
4. 享受温暖的夜间阅读体验！🌙

## 📁 手动安装（备选方案）

如果上述方法不工作，您可以手动找到主题文件夹：

**macOS:**
```
~/Library/Application Support/abnerworks/Typora/themes/
```

**Windows:**
```
%APPDATA%\Typora\themes\
```
或
```
C:\Users\[用户名]\AppData\Roaming\Typora\themes\
```

**Linux:**
```
~/.config/Typora/themes/
```

将 `claude-anthropic-dark.css` 文件复制到上述目录，然后重启 Typora。

## 🎨 同时安装浅色和暗色版本

如果您想同时拥有两个版本：

1. 复制 `claude-anthropic.css` 到主题文件夹
2. 复制 `claude-anthropic-dark.css` 到主题文件夹
3. 重启 Typora
4. 现在您可以在主题列表中选择：
   - **Claude Anthropic** (浅色版)
   - **Claude Anthropic Dark** (暗色版)

### 快速切换技巧

**方法 1：手动切换**
- 随时在 Typora 偏好设置中切换主题

**方法 2：系统级自动切换**（推荐）
- macOS: 系统偏好设置 → 通用 → 外观 → 自动
- Windows: 设置 → 个性化 → 颜色 → 选择默认应用模式
- 主题会根据系统设置自动切换（如果 CSS 中包含媒体查询）

## 🔧 故障排除

### 问题 1：主题列表中看不到 "Claude Anthropic Dark"

**解决方案：**
1. 确认文件名完全正确：`claude-anthropic-dark.css`
2. 确认文件已复制到正确的主题文件夹
3. 完全关闭并重新启动 Typora
4. 检查文件权限（确保 Typora 可以读取）

### 问题 2：主题显示但样式不正确

**解决方案：**
1. 清除 Typora 缓存（重启通常足够）
2. 检查是否有其他 CSS 文件冲突
3. 确保使用的是最新版本的 Typora
4. 尝试重新下载主题文件

### 问题 3：暗色模式不自动切换

**解决方案：**
1. 确认操作系统已启用暗色模式
2. 检查系统时间（某些系统在日落后自动切换）
3. 手动在 Typora 中选择暗色主题
4. 注意：当前暗色版本是独立主题，不是通过媒体查询自动切换

### 问题 4：字体显示不正确

**解决方案：**
1. 主题使用系统回退字体：
   - Serif: Georgia → Times New Roman → serif
   - Sans: Arial → system-ui → sans-serif
   - Mono: SF Mono → Monaco → Consolas → monospace
2. 确保系统安装了这些字体
3. 如果想使用自定义字体，编辑 CSS 文件中的 `--font-*` 变量

## 💡 高级配置

### 自定义暗色主题

您可以编辑 `claude-anthropic-dark.css` 文件来微调主题：

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

### 创建自己的变体

1. 复制 `claude-anthropic-dark.css` 为新文件（如 `my-custom-dark.css`）
2. 修改 CSS 变量
3. 在文件顶部更新主题名称注释
4. 重启 Typora 并选择新主题

## 📊 验证安装

安装成功后，您应该看到：

✅ Typora 背景变为深暖色调 (#141413)  
✅ 标题使用衬线字体，颜色为象牙白 (#faf9f5)  
✅ 正文使用无衬线字体，颜色为暖银色 (#b0aea5)  
✅ 代码块背景为深炭色 (#30302e)  
✅ 引用块左侧有赤陶色边框 (#c96442)  
✅ 链接显示为珊瑚色 (#d97757)  

## 🎯 最佳实践

### 环境设置
- 🕯️ 在昏暗环境中使用暗色主题效果最佳
- 💡 降低屏幕亮度以配合暗色主题
- 👁️ 启用系统的夜览/护眼模式获得更好体验

### 工作流程
- 📝 长时间写作时使用暗色主题减少眼部疲劳
- 🌙 夜间工作时切换到暗色版本
- 🔄 根据时间和环境光在两个版本间切换

### 团队协作
- 📤 导出 PDF/HTML 时注意当前使用的主题
- 📸 分享截图时注明使用的主题版本
- 🎨 团队项目中统一主题以保持文档一致性

## 📚 相关资源

- [暗色主题详细说明](README-DARK.md) - 完整的设计规范
- [主题对比指南](THEME_COMPARISON.md) - 浅色 vs 暗色详细对比
- [主 README](README.md) - 项目总览
- [快速参考](QUICK_REFERENCE.md) - 常用样式速查

## ❓ 常见问题

**Q: 暗色版本会自动跟随系统暗色模式吗？**  
A: 当前版本是独立的暗色主题，需要手动选择。如需自动切换，可以同时安装两个版本并使用系统级主题切换工具。

**Q: 我可以修改主题的颜色吗？**  
A: 当然可以！编辑 CSS 文件中的 `:root` 变量部分即可自定义颜色。

**Q: 暗色版本会影响导出的 PDF 吗？**  
A: 是的，导出的 PDF 会反映当前激活的主题样式。

**Q: 两个版本可以同时激活吗？**  
A: 不可以，Typora 一次只能激活一个主题。但您可以快速切换。

**Q: 暗色版本在所有操作系统上都一样吗？**  
A: 是的，CSS 主题在不同平台上表现一致，只依赖 Typora 的渲染引擎。

## 🆘 获取帮助

如果遇到其他问题：

1. 查看 [GitHub Issues](https://github.com/yourusername/typora-theme-claude-anthropic/issues)
2. 搜索是否已有类似问题的解答
3. 如果没有，创建新的 Issue 并描述您的问题
4. 附上：
   - Typora 版本
   - 操作系统版本
   - 问题截图
   - 重现步骤

## 🎉 开始使用

安装完成后，打开任意 Markdown 文件，享受温暖、舒适的夜间写作体验！

**祝您写作愉快！** ✍️🌙✨

---

*提示：查看 [THEME_COMPARISON.md](THEME_COMPARISON.md) 了解何时使用浅色版本，何时使用暗色版本的建议。*

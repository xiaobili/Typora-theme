# Installation Guide - Claude Anthropic Theme

## 📋 Prerequisites 前置要求

- Typora (最新版本推荐)
- 操作系统：macOS / Windows / Linux

---

## 🚀 Quick Install 快速安装

### Step 1: Download the Theme

确保您已下载 `claude-anthropic.css` 文件。

### Step 2: Open Typora Theme Folder

**macOS:**
1. 打开 Typora
2. 点击菜单栏 **Typora** → **Preferences** (或按 `Cmd + ,`)
3. 选择 **Appearance** 标签
4. 点击 **Open Theme Folder** 按钮

**Windows:**
1. 打开 Typora
2. 点击 **File** → **Preferences** (或按 `Ctrl + ,`)
3. 选择 **Appearance** 标签
4. 点击 **Open Theme Folder** 按钮

**Linux:**
1. 打开 Typora
2. 点击 **File** → **Preferences**
3. 选择 **Appearance** 标签
4. 点击 **Open Theme Folder** 按钮

### Step 3: Copy Theme File

将 `claude-anthropic.css` 文件复制到打开的主题文件夹中。

### Step 4: Restart Typora

完全关闭并重新打开 Typora。

### Step 5: Activate the Theme

1. 打开 **Preferences** → **Appearance**
2. 在 **Theme** 下拉菜单中选择 **Claude Anthropic**
3. 主题立即生效！

---

## 🔍 Verify Installation 验证安装

打开 `preview.md` 文件检查主题是否正确应用：

1. 在 Typora 中打开 `preview.md`
2. 确认看到温暖的羊皮纸背景（不是纯白）
3. 标题应该使用衬线字体（类似 Georgia）
4. 引用块应该有左侧的赤陶色边框

如果一切正常，恭喜！主题已成功安装。✅

---

## ⚙️ Optional Configuration 可选配置

### Enable Dark Mode 启用暗色模式

主题支持系统级暗色模式：

**macOS:**
- System Preferences → General → Appearance → Dark

**Windows:**
- Settings → Personalization → Colors → Choose your color → Dark

**Linux:**
取决于您的桌面环境，通常在系统设置的外观选项中。

### Custom Font Installation 自定义字体安装（可选）

如果您想获得最佳效果，可以安装 Anthropic 的自定义字体：

1. **Anthropic Serif** - 用于标题
2. **Anthropic Sans** - 用于正文
3. **Anthropic Mono** - 用于代码

*注意：这些是 Anthropic 的专有字体，可能不公开可用。主题已配置了良好的回退字体（Georgia, Arial, SF Mono）。*

---

## 🎨 Customization 自定义主题

### Method 1: Edit CSS Variables

编辑 `claude-anthropic.css` 文件的 `:root` 部分：

```css
:root {
  /* Change background color */
  --parchment: #f5f4ed;  /* Try: #faf8f3 for lighter, #edebe4 for darker */
  
  /* Change accent color */
  --terracotta-brand: #c96442;  /* Try: #d4754f for lighter, #b8543a for darker */
  
  /* Adjust base font size */
  font-size: 16px;  /* Try: 15px for smaller, 17px for larger */
}
```

### Method 2: Adjust Spacing

修改间距变量：

```css
:root {
  --space-base: 8px;  /* Increase for more spacing, decrease for compact */
}
```

### Method 3: Modify Border Radius

调整圆角大小：

```css
:root {
  --radius-comfortable: 8px;   /* Buttons and cards */
  --radius-generous: 12px;     /* Primary buttons */
  --radius-very: 16px;         /* Featured containers */
}
```

---

## 🐛 Troubleshooting 故障排除

### Theme Not Appearing in List

**问题：** 主题没有出现在 Typora 的主题列表中

**解决方案：**
1. 确认文件名是 `claude-anthropic.css`（不是 `.txt` 或其他扩展名）
2. 确认文件位于正确的主题文件夹中
3. 完全重启 Typora（不仅仅是关闭窗口）
4. 检查文件权限（应该是可读的）

### Fonts Look Different

**问题：** 字体看起来与预览不同

**说明：**
- 主题使用系统回退字体（Georgia, Arial, SF Mono）
- 如果您没有安装 Anthropic 自定义字体，这是正常的
- 整体布局和颜色应该仍然正确

### Colors Seem Off

**问题：** 颜色看起来不正确

**解决方案：**
1. 检查是否启用了系统的色彩配置文件
2. 尝试在不同的显示器上查看
3. 确认没有其他主题覆盖样式

### Code Blocks Not Styled

**问题：** 代码块没有正确的样式

**解决方案：**
1. 确保使用 Typora 的代码块语法（```language）
2. 尝试重启 Typora
3. 检查是否有其他插件冲突

---

## 📱 Mobile Usage 移动端使用

Typora 目前没有官方移动应用，但您可以在以下平台使用：

- **iPad**: 通过 Sidecar 或远程桌面
- **Android/iOS**: 通过云同步在其他设备上编辑

主题在这些平台上会自动响应屏幕尺寸。

---

## 🔄 Updates 更新主题

当主题有新版本时：

1. 下载新的 `claude-anthropic.css` 文件
2. 替换主题文件夹中的旧文件
3. 重启 Typora

*提示：如果您进行了自定义修改，请先备份您的版本。*

---

## 💡 Tips & Best Practices 使用技巧

### For Best Reading Experience

1. **Use Headings Hierarchically**: H1 → H2 → H3 for clear structure
2. **Add Blockquotes**: Highlight key insights with the distinctive left border
3. **Include Code Blocks**: Technical content looks great in dark-themed code blocks
4. **Use Tables**: Compare information with clean, bordered tables
5. **Add Images**: Rounded corners make images feel integrated

### Writing Workflow

1. Start with an H1 title
2. Add metadata in YAML front matter (optional)
3. Use H2 for major sections
4. Use H3 for subsections
5. Sprinkle blockquotes for emphasis
6. End with a conclusion

### Keyboard Shortcuts

- `Cmd/Ctrl + B`: Bold
- `Cmd/Ctrl + I`: Italic
- `Cmd/Ctrl + K`: Insert link
- `` Cmd/Ctrl + Alt + C ``: Insert code block
- `Cmd/Ctrl + Shift + Q`: Insert blockquote

---

## 📞 Support 获取帮助

如果您遇到问题：

1. 查看本安装指南的故障排除部分
2. 检查 Typora 的官方文档
3. 查看主题 GitHub 仓库的 Issues（如果有）
4. 联系 Typora 支持团队

---

## 🎉 You're All Set!

Enjoy your warm, editorial writing experience with the Claude Anthropic theme! ✍️📚

**Happy Writing!**

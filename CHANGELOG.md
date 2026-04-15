# Changelog - Claude Anthropic Typora Theme

所有重要的项目更改都将记录在此文件中。

格式基于 [Keep a Changelog](https://keepachangelog.com/)，版本遵循 [Semantic Versioning](https://semver.org/)。

---

## [Unreleased]

### ✨ Added - 新增功能

#### 暗色主题版本 (v1.0.0)
- ✅ 完整的暗色版本主题文件 `claude-anthropic-dark.css`
- ✅ 基于 Deep Dark (#141413) 的温暖深色调背景
- ✅ Dark Surface (#30302e) 卡片和容器表面
- ✅ Ivory (#faf9f5) 主要文本颜色
- ✅ Warm Silver (#b0aea5) 次要文本和元数据
- ✅ 保持 exclusively 暖色调中性色（无冷蓝灰色）
- ✅ 暗色版本的独立 package.json 配置
- ✅ 完整的暗色主题文档体系

#### 文档更新
- ✅ `README-DARK.md` - 暗色主题详细说明
- ✅ `THEME_COMPARISON.md` - 浅色与暗色版本详细对比
- ✅ `INSTALL-DARK.md` - 暗色主题安装指南
- ✅ 更新主 `README.md` 添加双主题介绍
- ✅ 添加主题切换建议和最佳实践

#### 色彩系统（暗色版）
- ✅ 页面背景: #141413 (Deep Dark)
- ✅ 卡片表面: #30302e (Dark Surface)
- ✅ 主要文本: #faf9f5 (Ivory)
- ✅ 次要文本: #b0aea5 (Warm Silver)
- ✅ 代码块背景: #30302e (Dark Surface)
- ✅ 边框系统: 温暖的深色调变体
- ✅ 环状阴影: 暗色版本适配

---

## [1.0.0] - 2026-04-15

### ✨ Added - 新增功能

#### 核心主题
- ✅ 完整的 Claude 设计系统实现
- ✅ 温暖的羊皮纸色调 (#f5f4ed) 作为主背景
- ✅ 独家暖色调中性色系统（无冷蓝灰色）
- ✅ Terracotta 品牌色 (#c96442) 作为主要强调色
- ✅ CSS 变量系统便于自定义

#### 排版系统
- ✅ Serif/Sans 字体分层（标题用衬线体，正文用无衬线体）
- ✅ 完整的标题层次（H1-H6，64px-20px）
- ✅ 杂志级行高（正文 1.60）
- ✅ 统一的标题字重（500）
- ✅ 响应式字号调整

#### 组件样式
- ✅ 链接样式（温暖下划线，悬停变赤陶色）
- ✅ 强调文本（粗体、斜体、删除线、高亮）
- ✅ 行内代码和代码块（深色背景 + 暖银色文字）
- ✅ 引用块（左侧赤陶色边框 + 象牙白背景）
- ✅ 列表（有序、无序、任务列表）
- ✅ 表格（温暖边框 + 悬停效果）
- ✅ 图片（圆角 + 说明文字）
- ✅ 分隔线（温暖奶油色）
- ✅ 脚注（底部组织显示）
- ✅ 数学公式支持
- ✅ 图表容器样式

#### UI 组件
- ✅ 侧边栏样式（温暖背景 + 活动项高亮）
- ✅ 大纲面板（活跃项赤陶色标记）
- ✅ 搜索面板（焦点环蓝色）
- ✅ 按钮样式（次要、主要、暗色变体）

#### 高级功能
- ✅ 环状阴影系统（0px 0px 0px 1px）
- ✅ 滚动条美化（温暖色调）
- ✅ 打印样式优化
- ✅ 响应式设计（移动端适配）
- ✅ 暗色模式支持（系统级别自动切换）
- ✅ 选中文本样式

#### 文档套件
- ✅ README.md - 主题介绍和使用说明
- ✅ INSTALL.md - 详细安装指南（多平台）
- ✅ QUICK_START.md - 3 步快速启动指南
- ✅ QUICK_REFERENCE.md - 设计师/开发者速查表
- ✅ preview.md - 完整样式预览文档
- ✅ PROJECT_STRUCTURE.md - 项目结构详解
- ✅ package.json - 主题配置和元数据
- ✅ CHANGELOG.md - 变更日志（本文件）

### 🎨 Design Features - 设计特色

#### 色彩系统
- 主背景：Parchment (#f5f4ed)
- 卡片背景：Ivory (#faf9f5)
- 主要文字：Near Black (#141413)
- 次要文字：Olive Gray (#5e5d59)
- 强调色：Terracotta (#c96442)
- 边框：Border Cream (#f0eee6)
- 完全避免冷蓝灰色

#### 间距系统
- 基于 8px 基础单位
- 10 级间距：3px, 4px, 6px, 8px, 10px, 12px, 16px, 20px, 24px, 30px
-  editorial 节奏的 section 间距

#### 圆角系统
- 7 级圆角：4px, 6px, 8px, 12px, 16px, 24px, 32px
- 有机、亲切的感觉

#### 阴影哲学
- Level 0: Flat（无阴影）
- Level 1: Contained（边框）
- Level 2: Ring（环状阴影）
- Level 3: Whisper（柔和投影）
- Level 4: Inset（内阴影）

### 📱 Responsive Design - 响应式设计

#### 断点
- Small Mobile: <479px
- Mobile: 479-640px
- Large Mobile: 640-767px
- Tablet: 768-991px
- Desktop: 992px+

#### 自适应特性
- 标题字号渐进缩小
- Section padding 比例缩减
- 导航折叠为汉堡菜单（Typora UI）
- 多列布局堆叠为单列
- 保持 editorial 节奏

### 🌙 Dark Mode - 暗色模式

- 系统级别自动检测
- 保持温暖色调的同时减少眼部疲劳
- 所有组件都有暗色变体
- 无缝切换体验

### 🔧 Customization - 可定制性

- CSS 变量系统
- 易于修改颜色
- 可调整间距
- 可自定义圆角
- 清晰的代码注释

### 📚 Documentation - 文档质量

- 详细的安装指南（3 个平台）
- 故障排除部分
- 快速参考卡片
- 完整样式预览
- 设计原则说明
- 最佳实践建议
- 自定义教程

### 🎯 Best Practices - 最佳实践

- ✅ 使用 Parchment 作为主背景
- ✅ 保持所有中性色温暖
- ✅ Serif 标题统一使用 500 字重
- ✅ 正文使用 1.60 宽松行高
- ✅ 交互状态使用环状阴影
- ✅ Light/Dark section 交替创造节奏
- ✅ generous 圆角（8-32px）

### ❌ Anti-Patterns - 避免的模式

- ❌ 不使用冷蓝灰色
- ❌ Serif 标题不使用 bold (700+)
- ❌ 不引入饱和色（除 Terracotta）
- ❌ 不使用锐角（<6px）
- ❌ 不使用重投影
- ❌ 不使用纯白作为页面背景
- ❌ 正文字行高不低于 1.40

---

## [Unreleased] - 待发布

### 🚀 Planned Features - 计划功能

#### Short-term (v1.1.0)
- [ ] 更多代码语言高亮样式优化
- [ ] Mermaid 图表样式增强
- [ ] 添加平滑过渡动画
- [ ] 改进数学公式渲染
- [ ] 优化打印样式

#### Mid-term (v1.2.0)
- [ ] 主题生成器工具（在线自定义）
- [ ] 更多预设配色方案
- [ ] 示例模板库
- [ ] 视频教程
- [ ] 社区贡献指南

#### Long-term (v2.0.0)
- [ ] 支持 Typora 插件系统
- [ ] 动态主题切换
- [ ] 用户偏好保存
- [ ] 云端同步配置
- [ ] 主题市场集成

### 🐛 Known Issues - 已知问题

目前没有已知问题。

### 💡 Suggestions Welcome - 欢迎建议

如果您有任何功能建议或改进意见，请在 GitHub Issues 中提出！

---

## Version History Summary

| Version | Date | Status | Key Features |
|---------|------|--------|--------------|
| 1.0.0 | 2026-04-15 | ✅ Released | Initial release, complete design system |
| Unreleased | - | 🚧 In Development | Planned enhancements |

---

## Migration Guide - 迁移指南

### From v0.x to v1.0.0

这是首个正式版本，无需迁移。

### Future Versions

未来版本更新时：
1. 备份您的自定义修改（如果有）
2. 下载新版本
3. 替换 `claude-anthropic.css` 文件
4. 重启 Typora
5. 检查变更日志了解新功能

---

## Credits - 致谢

### Design Inspiration
- **Claude by Anthropic** - 原始设计系统和视觉语言
- Website: https://www.anthropic.com/claude

### Technology
- **Typora** - 优秀的 Markdown 编辑器
- Website: https://typora.io/

### Standards & Guidelines
- [Keep a Changelog](https://keepachangelog.com/)
- [Semantic Versioning](https://semver.org/)
- [CSS Custom Properties](https://developer.mozilla.org/en-US/docs/Web/CSS/--*)

---

## Contributing - 贡献

欢迎贡献！请：
1. Fork 本仓库
2. 创建特性分支
3. 提交更改
4. 开启 Pull Request
5. 更新此变更日志

详见 [PROJECT_STRUCTURE.md](PROJECT_STRUCTURE.md) 的贡献指南部分。

---

**Thank you for using Claude Anthropic Typora Theme!** ✍️📚

*Last updated: 2026-04-15*

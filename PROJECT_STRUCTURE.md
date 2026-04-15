# 📁 项目结构 - Claude Anthropic Typora Theme

本文档说明项目的文件组织和结构，包含浅色和暗色双版本主题。

## 📁 当前项目结构

```
Typora-theme/
│
├── 🎨 主题文件
│   ├── claude-anthropic.css          # 浅色版本主题（羊皮纸色调）
│   └── claude-anthropic-dark.css     # 暗色版本主题（深暖色调）✨ NEW
│
├── 📦 配置文件
│   ├── package.json                  # 浅色版本配置
│   └── package-dark.json             # 暗色版本配置 ✨ NEW
│
├── 📖 主要文档
│   ├── README.md                     # 项目总览（已更新双主题信息）✨ UPDATED
│   ├── INSTALL.md                    # 浅色版本安装指南
│   └── INSTALL-DARK.md               # 暗色版本安装指南 ✨ NEW
│
├── 📚 详细文档
│   ├── README-DARK.md                # 暗色版本详细说明 ✨ NEW
│   ├── THEME_COMPARISON.md           # 主题对比指南 ✨ NEW
│   ├── DESIGN_SYSTEM_INSPIRED_BY_CLAUDE.md  # 设计系统灵感来源
│   ├── LIST_STYLES.md                # 列表样式说明
│   └── CODE_BLOCK_UPDATE.md          # 代码块更新说明
│
├── ⚡ 快速参考
│   ├── QUICK_START.md                # 快速开始指南
│   ├── QUICK_REFERENCE.md            # 浅色版快速参考
│   └── QUICK_REFERENCE-DARK.md       # 暗色版快速参考 ✨ NEW
│
├── 📝 变更记录
│   ├── CHANGELOG.md                  # 版本历史（已更新）✨ UPDATED
│   └── SUMMARY.md                    # 项目总结
│
└── 🧪 测试文件
    └── preview.md                    # 主题预览测试文件
```

---

## 🆕 新增文件说明（暗色版本）

### 核心文件

#### 1. `claude-anthropic-dark.css`
**类型**: CSS 主题文件  
**用途**: 暗色版本的完整主题样式  
**特点**:
- 基于 Deep Dark (#141413) 的温暖深色调
- 完整的排版系统和组件样式
- 保持 exclusively 暖色调中性色
- 独立的 CSS 变量定义

**关键色彩**:
```css
--parchment: #141413;      /* 页面背景 */
--ivory: #30302e;          /* 卡片表面 */
--charcoal-warm: #b0aea5;  /* 主要文本 */
--terracotta-brand: #c96442; /* 品牌强调色 */
```

#### 2. `package-dark.json`
**类型**: JSON 配置文件  
**用途**: 暗色主题的元数据配置  
**内容**:
- 主题名称: "Claude Anthropic Dark"
- 版本: 1.0.0
- 标签: dark, warm, editorial, serif
- 依赖关系指向主仓库

**使用方法**: 
如需使用此配置，重命名为 `package.json` 并与 CSS 文件一起安装。

### 文档文件

#### 3. `README-DARK.md`
**类型**: Markdown 文档  
**用途**: 暗色主题的完整说明文档  
**内容包括**:
- 设计特色和核心理念
- 完整的色彩系统表格
- 排版层次规范
- 组件样式详解
- 安装方法（两种）
- 与浅色版本对比表
- 设计原则（Do's & Don'ts）
- 响应式设计说明
- 版权和技术支持信息

**目标读者**: 
- 想要了解暗色主题设计理念的用户
- 需要详细技术规范的开发者
- 考虑在两个版本间选择的团队

#### 4. `THEME_COMPARISON.md`
**类型**: Markdown 对比文档  
**用途**: 详细对比浅色和暗色版本  
**内容包括**:
- 完整的色彩对照表（背景、文本、边框、代码、表格等）
- 共同特征说明（排版、间距、圆角、组件行为）
- 设计哲学对比（"温暖羊皮纸" vs "温暖深夜书房"）
- 技术实现差异（CSS 变量映射）
- 选择建议（何时使用哪个版本）
- 安装和切换技巧
- 最佳实践指南

**目标读者**:
- 犹豫选择哪个版本的用户
- 需要向团队解释差异的项目经理
- 想要同时安装两个版本的用户

#### 5. `INSTALL-DARK.md`
**类型**: Markdown 安装指南  
**用途**: 逐步指导暗色主题安装  
**内容包括**:
- 前置要求清单
- 快速安装（3 步完成）
- 手动安装备选方案
- 同时安装两个版本的方法
- 故障排除（4 个常见问题）
- 高级配置和自定义
- 验证安装成功的检查清单
- 最佳实践和环境设置建议
- 常见问题解答（FAQ）

**目标读者**:
- 首次安装暗色主题的用户
- 遇到安装问题的用户
- 想要自定义主题的高级用户

#### 6. `QUICK_REFERENCE-DARK.md`
**类型**: Markdown 快速参考  
**用途**: 暗色主题的色彩和样式速查卡片  
**内容包括**:
- 核心色彩代码片段（可直接复制）
- 排版规范表格
- 组件样式速查（代码块、引用块、表格、列表、链接）
- 间距系统数值
- 圆角系统层级
- 设计原则摘要
- 响应式断点
- CSS 变量自定义示例
- 使用场景建议
- 快速安装命令

**目标读者**:
- 需要快速查阅色彩值的开发者
- 正在自定义主题的用户
- 需要参考规范的团队成员

### 更新的文件

#### 7. `README.md` (已更新)
**变更内容**:
- ✅ 添加双主题介绍区块
- ✅ 列出两个可用主题及其特点
- ✅ 添加浅色/暗色版本特性对比
- ✅ 更新特色功能描述（移除单一背景色描述）
- ✅ 添加相关文档链接
- ✅ 更新页脚标语

**新增章节**:
- "📦 可用主题" - 介绍两个版本
- "🌗 双主题支持" - 详细的色彩对比
- "📚 相关文档" - 文档导航

#### 8. `CHANGELOG.md` (已更新)
**变更内容**:
- ✅ 添加 [Unreleased] 区块
- ✅ 记录暗色版本的所有新增功能
- ✅ 列出新增的文档文件
- ✅ 详细说明暗色版本的色彩系统

**新增条目**:
- 暗色主题版本 (v1.0.0)
- 文档更新清单
- 色彩系统（暗色版）详细说明

---

## 📊 文件统计

### 按类型分类

| 类型 | 数量 | 文件列表 |
|------|------|---------|
| CSS 主题 | 2 | claude-anthropic.css, claude-anthropic-dark.css |
| JSON 配置 | 2 | package.json, package-dark.json |
| Markdown 文档 | 13 | README, INSTALL, CHANGELOG 等 |
| 测试文件 | 1 | preview.md |
| **总计** | **18** | - |

### 按版本分类

| 版本 | 专属文件 | 共享文件 |
|------|---------|---------|
| 浅色版 | claude-anthropic.css, package.json, INSTALL.md, QUICK_REFERENCE.md | README.md, CHANGELOG.md, 设计文档等 |
| 暗色版 | claude-anthropic-dark.css, package-dark.json, INSTALL-DARK.md, README-DARK.md, QUICK_REFERENCE-DARK.md | README.md, CHANGELOG.md, 设计文档等 |
| 通用 | - | THEME_COMPARISON.md, 设计系统文档, preview.md |

---

## 🎯 文件使用指南

### 对于普通用户

**只想使用主题？**
1. 阅读 `README.md` 了解项目
2. 查看 `THEME_COMPARISON.md` 选择版本
3. 根据选择阅读对应的安装指南：
   - 浅色版: `INSTALL.md`
   - 暗色版: `INSTALL-DARK.md`
4. 复制对应的 CSS 文件到 Typora 主题文件夹
5. 重启 Typora 并启用主题

**需要快速参考？**
- 浅色版: `QUICK_REFERENCE.md`
- 暗色版: `QUICK_REFERENCE-DARK.md`

### 对于开发者

**想要自定义主题？**
1. 阅读对应版本的详细说明：
   - 浅色版: `README.md` 中的设计原则部分
   - 暗色版: `README-DARK.md`
2. 查看 `DESIGN_SYSTEM_INSPIRED_BY_CLAUDE.md` 了解设计规范
3. 编辑 CSS 文件中的 `:root` 变量
4. 参考 `QUICK_REFERENCE*.md` 中的色彩值

**想要贡献代码？**
1. 阅读所有文档了解项目结构
2. 查看 `CHANGELOG.md` 了解历史变更
3. 遵循现有的代码风格和命名规范
4. 提交 PR 时更新相关文档

### 对于团队管理者

**需要在团队中推广？**
1. 分享 `THEME_COMPARISON.md` 帮助团队成员选择
2. 根据团队工作环境推荐合适的版本
3. 建立内部的主题使用规范
4. 统一导出文档的主题版本

---

## 🔄 版本演进

### v1.0.0 (2026-04-15)
- ✅ 初始浅色版本发布
- ✅ 完整的 Claude 设计系统实现
- ✅ 基础文档体系

### v1.1.0 (计划中 - 暗色版本)
- ✅ 完整的暗色版本实现
- ✅ 扩展的文档体系
- ✅ 主题对比指南
- ⏳ 可能添加自动切换功能

### 未来规划
- 📋 可能的中等色调版本
- 📋 高对比度无障碍版本
- 📋 更多自定义变体
- 📋 Typora 主题市场提交

---

## 📝 文档维护

### 更新原则
1. **同步更新**: 修改 CSS 时必须更新相关文档
2. **版本控制**: 所有变更记录在 CHANGELOG.md
3. **交叉引用**: 相关文档之间互相链接
4. **用户导向**: 文档以用户需求为中心组织

### 文档优先级
1. 🔴 高: README.md, INSTALL*.md - 用户首先看到
2. 🟡 中: README-DARK.md, THEME_COMPARISON.md - 深入了解
3. 🟢 低: QUICK_REFERENCE*.md - 日常参考

### 翻译计划
目前所有文档均为中文。未来可能添加：
- English (英文)
- 日本語 (日文)
- 한국어 (韩文)

---

## 🆘 获取帮助

**找不到需要的信息？**
1. 搜索所有 Markdown 文件
2. 查看 GitHub Issues
3. 创建新的 Issue 提问
4. 联系维护者

**发现文档错误？**
1. 提交 Issue 报告问题
2. 或直接提交 PR 修正
3. 注明具体文件和行号

---

**最后更新**: 2026-04-15  
**文档版本**: 1.1.0  
**维护者**: Claude Anthropic Theme Team

*保持文档与代码同步更新！* 📚✨

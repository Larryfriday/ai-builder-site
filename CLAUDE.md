# 项目规范

## 技术栈

- **框架**: 纯 HTML/CSS/JS (无框架)
- **语言**: HTML5, CSS3, JavaScript
- **部署**: 静态网站托管

## 开发规范

### 代码风格

- 使用 CSS 变量定义颜色主题
- 采用深色主题 (背景 #0a0a0f, 强调色 #00d4ff)
- 移动端优先的响应式设计
- 使用 clamp() 实现流体排版

### 提交规范

遵循 Conventional Commits:
- `feat:` 新功能
- `fix:` Bug 修复
- `docs:` 文档更新
- `style:` 样式调整
- `refactor:` 代码重构

### 分支策略

- `main` - 生产分支
- `master` - 开发分支 (当前)

## 项目结构

```
/Users/jerome/my-first-website/
├── index.html         # 主页面
├── .claude/
│   └── settings.local.json  # Claude 本地配置
├── .git/
└── CLAUDE.md          # 项目规范 (本文件)
```

## 常用命令

### 开发

直接在浏览器中打开 index.html，或使用 VS Code / Cursor 的 Live Server 插件。

### Git 操作

```bash
# 查看状态
git status

# 添加更改
git add .

# 提交
git commit -m "feat: 添加新功能"

# 推送到远程
git push origin master
```

## Cursor + Claude Code 工作流

### 1. Cursor 编辑器

- `Cmd+K` - 快速 AI 询问
- `Cmd+L` - 侧边栏对话
- `Tab` - 接受 AI 建议

### 2. Claude Code CLI

```bash
# 分析项目
claude "分析这个网站的结构"

# 代码审查
claude "审查 index.html 的代码质量"
```

### 3. 插件使用

- GitHub: `claude mcp__plugin_github_github__...`
- 搜索技能: `claude search-first:...`
- TDD: `claude tdd-workflows:...`

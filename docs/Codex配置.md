# Codex 配置

Codex 通常会读取当前项目或全局的 `AGENTS.md`。

## 推荐做法

把下面内容加入 Codex 全局或项目入口：

```text
主 AI 记忆库：
<你的 Obsidian vault 路径>/Agent记忆库

开始重要任务前优先读取：
<你的 Obsidian vault 路径>/Agent记忆库/说明.md
<你的 Obsidian vault 路径>/Agent记忆库/AGENTS.md
```

如果任务涉及项目上下文，读取：

```text
AI记忆/30_项目记忆/<状态>/<项目名>/_项目记忆/00-关键上下文.md
AI记忆/30_项目记忆/<状态>/<项目名>/_项目记忆/99-索引.md
```


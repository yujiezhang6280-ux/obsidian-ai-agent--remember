# Claude 配置

Claude 不一定会自动读取 Codex 的 `AGENTS.md`，所以需要单独把 Obsidian 入口接入 Claude。

## 推荐做法

在 Claude 的项目或全局说明中加入：

```text
请先读取：
<你的 Obsidian vault 路径>/Agent记忆库/CLAUDE.md

以后所有记忆读取和项目记忆沉淀，都以这个 Obsidian Agent 记忆库为主入口。
```

## 权限注意

如果 Claude 报：

```text
Path is outside allowed working directories
```

说明 Claude 当前没有权限读取 Obsidian 路径。需要在 Claude 中允许该路径，或把 Claude 的工作目录设置到 Obsidian 记忆库。


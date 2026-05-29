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

## 项目记忆兼容

Claude 不需要安装 Codex 的私有 Skill。只要它按 `CLAUDE.md` 入口读取，并把项目记忆写入中文 `_项目记忆/` 结构即可。

项目记忆支持：

```text
AI记忆/30_项目记忆/<状态>/<独立项目>/_项目记忆/
AI记忆/30_项目记忆/<状态>/<项目组>/<项目名>/_项目记忆/
```

没有 `_项目记忆/` 的中间目录是项目组容器，应继续向下一层查找，不要把项目事实写在容器目录。

如果旧文档提到 `_project_memory/`、`00-critical.md`、`parents.md` 或 `99-index.md`，按 `AI记忆/30_项目记忆/说明.md` 的映射处理。

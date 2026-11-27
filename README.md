# Agent Tutor v0.2.1 · 本地 Agent 新手陪练

用你手头的本地 Agent 开始练习。Agent Tutor 会先理解目标，再带你完成一小步、核对结果。

任务完成后，可按需沉淀为本地/Obsidian 笔记、复用 Prompt 或自己的小 Skill。

[第一次使用？打开带 Codex 官方界面图的逐步教程](docs/QUICKSTART.md)。

**选一种就好。第一次来，直接用方法一。**

## 方法一｜一句话让你的 Agent 自己装（最推荐，全平台通用）

不用手动找 `.agents` 或 `.claude` 这类隐藏文件夹。打开你正在用的本地 Agent（Codex、Claude Code、AGY、ZCode 等），直接复制下面**任意一句**发给它，遇到权限确认点「允许」即可：

**能直接连 GitHub 时，复制这句：**

```text
请帮我从 https://github.com/Loku1210/agent-tutor（版本 v0.2.1）下载并安装里面的 agent-tutor Skill（路径在 practice/.agents/skills/agent-tutor）到你支持的 Skills 目录。装好后直接读取它的 SKILL.md，带我开始第一次新手对话。
```

**连不上 GitHub 时，先下载 [Agent-Tutor-v0.2.1.zip](https://github.com/Loku1210/agent-tutor/releases/download/v0.2.1/Agent-Tutor-v0.2.1.zip) 到电脑「下载」文件夹，再复制这句：**

```text
我刚把 Agent-Tutor-v0.2.1.zip 下载到电脑的「下载」文件夹了，请你帮我解压并把里面的 agent-tutor Skill 安装到你支持的 Skills 目录。装好后直接读取它的 SKILL.md，带我开始第一次新手对话。
```

> 小提示：部分客户端装完新 Skill 后，要**新开一个会话**才会出现在技能列表里；按上面这句话，当前对话就能先直接带你体验一遍。

启动陪练后发「你好」，就能从四类练习中选一项：**1 办公与整理、2 科研与文献、3 日常与自学、4 文件与本地小工具**。回复数字即可，也可以直接说你手头想做的事。

## 方法二｜先用练习包试一次（Codex 零配置体验）

1. [下载练习包 ZIP](https://github.com/Loku1210/agent-tutor/releases/download/v0.2.1/Agent-Tutor-v0.2.1.zip)，然后解压。
2. 在 Codex 里新建本地项目，选择解压后的 **`practice` 文件夹**。详细图文步骤见[新手逐步教程](docs/QUICKSTART.md)。
3. 新开一个会话，发送 **你好**。如果没有进入陪练，再发送 **`$agent-tutor 你好`**。

也可以在 Codex 里直接用内置安装器安装到全局：

```text
$skill-installer 请从 https://github.com/Loku1210/agent-tutor/tree/v0.2.1/practice/.agents/skills/agent-tutor 安装 Agent Tutor
```

可以试试：**把示例笔记整理成待办，新建 todo.md，原文别动。**

想试科研场景？可以说：“我想了解阿尔茨海默病近年的单细胞和空间转录组研究。先帮我把检索范围、文献质量和交付内容问清楚，再整理成一段可执行的检索指令。”

## 方法三｜图形化导入或手动复制（前两种不适用时）

1. 下载并解压[练习包 ZIP](https://github.com/Loku1210/agent-tutor/releases/download/v0.2.1/Agent-Tutor-v0.2.1.zip)，找到里面的 `practice/.agents/skills/agent-tutor` 文件夹（看不到 `.agents` 时，macOS 在 Finder 按 `Command + Shift + .`，Windows 在资源管理器开启「隐藏的项目」）。
2. 按你的客户端导入或复制整个 `agent-tutor` 文件夹：

| 客户端 | 加载和启动 |
| --- | --- |
| Codex | 复制到个人目录下的 `.agents/skills/`（或直接打开 `practice` 文件夹），新开会话发送 `$agent-tutor 你好`。 |
| Claude Code | 复制到项目的 `.claude/skills/` 或个人的 `~/.claude/skills/`，新开会话输入 `/agent-tutor`。 |
| AGY（Antigravity） | 通过项目的 `.agents/skills/` 或客户端配置的 Skills 目录加载，再输入 `/agent-tutor` 或直接点名调用。 |
| ZCode | 通过项目的 `.zcode/skills/` / `.agents/skills/` 或用户级 `~/.zcode/skills/` 加载，输入 `/` 或 `$agent-tutor` 选择。 |
| WorkBuddy | 桌面版可在「专家·技能·连接器 → 技能 → 添加技能 → 上传技能」导入，从任务栏选择启动；企业版可用 `.codebuddy/skills/`。 |
| DeepSeek | 取决于本地客户端。支持 Skills 时通过加载器导入，否则将 `SKILL.md` 加入项目指令，并让客户端能读取 `references/` 和 `assets/`。 |

各客户端的目录和权限可能随版本而异，详见[客户端适配说明](practice/.agents/skills/agent-tutor/references/host-compatibility.md)与 [Codex 官方安装目录说明](https://learn.chatgpt.com/docs/build-skills#where-codex-loads-local-skills)。

## 没打开陪练？

装完后仍找不到时，**新开一个会话或重启客户端**再试一次；Codex 可显式发送 `$agent-tutor 你好`，Claude Code / AGY 可发送 `/agent-tutor`。

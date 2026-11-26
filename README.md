# Agent Tutor v0.1.0

这是一个 Codex 新手陪练。你可以只说一句想做的事，Tutor 会带你完成一个小任务，并告诉你怎么检查结果。

## 先试一次

1. 把 ZIP 完整解压到本机。打开 Codex，选择解压后的 `practice` 文件夹作为项目。
2. 在新会话里输入「你好」。Tutor 会问你今天想做什么。也可以直接输入 `$agent-tutor 你好`。
3. 想从样例开始，可以发送「把示例笔记整理成待办，新建一个文件，原件别改」。完成后，打开结果，挑一条跟原笔记核对。

练习项目已经附带 Skill。若 Codex 没看到它，请确认打开的是 `practice` 文件夹，且解压保留了其中的隐藏目录 `.agents`。必要时重启 Codex。

## 从 GitHub 安装

[下载练习 ZIP](https://github.com/Loku1210/agent-tutor/releases/tag/v0.1.0)，按上面的步骤体验。也可以在 Codex 中发送这一句，把 Tutor 安装给自己的项目使用：

```text
$skill-installer 请从 https://github.com/Loku1210/agent-tutor/tree/v0.1.0/practice/.agents/skills/agent-tutor 安装 Agent Tutor
```

安装完成后，新开一个 Codex 会话，输入 `$agent-tutor 你好`。

## 在自己的项目里用

把 `practice/.agents/skills/` 里的整个 `agent-tutor` 文件夹复制到个人目录下的 `.agents/skills`。没有这两个目录时，先创建。复制后，`SKILL.md` 应在个人目录下的 `.agents/skills/agent-tutor/` 内。

在 macOS Finder 中按 `Command + Shift + .` 可以显示隐藏文件夹。也可以在 PowerShell 或终端中查看。打开自己的项目并新建 Codex 会话，输入 `$agent-tutor 你好`，或用一句话说明你想做的事。

如果你只想在某个项目使用，就把 Skill 放到该项目的 `.agents/skills/agent-tutor/`。示例笔记和引导问候的项目规则留在练习目录即可。

[Codex 官方 Skill 说明](https://learn.chatgpt.com/docs/build-skills#where-codex-loads-local-skills)

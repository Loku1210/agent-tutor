# Agent Tutor · Codex 新手陪练

打开 Codex，说一句你想做的事。Agent Tutor 会先理解目标，再带你完成一小步、核对结果。

[第一次使用？打开带 Codex 官方界面图的逐步教程](docs/QUICKSTART.md)。

**选一种就好。第一次来，直接用方法一。**

## 方法一｜先试一次（推荐）

1. [下载练习包 ZIP](https://github.com/Loku1210/agent-tutor/releases/download/v0.1.0/Agent-Tutor-v0.1.0.zip)，然后解压。
2. 在 Codex 里新建本地项目，选择解压后的 **`practice` 文件夹**。详细图文步骤见[新手逐步教程](docs/QUICKSTART.md)。
3. 新开一个会话，发送 **你好**。如果没有进入陪练，再发送 **`$agent-tutor 你好`**。

陪练启动后，可以试试：**把示例笔记整理成待办，新建 todo.md，原文别动。**

想试科研场景？可以说：“我想了解阿尔茨海默病近年的单细胞和空间转录组研究。先帮我把检索范围、文献质量和交付内容问清楚，再整理成一段可执行的检索指令。”

## 方法二｜安装一次，在自己的项目里用

把下面整行复制到 Codex 聊天框，发送：

```text
$skill-installer 请从 https://github.com/Loku1210/agent-tutor/tree/v0.1.0/practice/.agents/skills/agent-tutor 安装 Agent Tutor
```

等 Codex 提示安装完成，打开你自己的项目，新开一个会话，发送 **`$agent-tutor 你好`**。逐步图解也在[新手教程](docs/QUICKSTART.md)。

## 方法三｜手动复制（前两种用不了时）

1. 下载并解压[练习包 ZIP](https://github.com/Loku1210/agent-tutor/releases/download/v0.1.0/Agent-Tutor-v0.1.0.zip)。
2. 找到 `practice/.agents/skills/agent-tutor`，复制整个 `agent-tutor` 文件夹。看不到 `.agents` 时，macOS 在 Finder 按 `Command + Shift + .`，Windows 在资源管理器中开启「隐藏的项目」。
3. 粘贴到个人目录下的 `.agents/skills`。如果目录还没有，就依次创建 `.agents` 和 `skills`。完成后，`SKILL.md` 应位于 `.agents/skills/agent-tutor` 里面。
4. 回到 Codex，新开一个会话，发送 **`$agent-tutor 你好`**。

[Codex 官方安装目录说明](https://learn.chatgpt.com/docs/build-skills#where-codex-loads-local-skills)

## 没打开陪练？

方法一先检查打开的是 `practice` 文件夹，再试 `$agent-tutor 你好`。方法二或三安装后仍找不到时，重启 Codex 再试一次。

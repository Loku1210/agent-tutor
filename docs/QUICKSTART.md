# 图文教程｜在 Codex 里第一次使用 Agent Tutor

这页带你从下载练习包，到在 Codex 里说出第一句话。图中界面直接使用 Codex 官方页面提供的真实界面图；下方项目名和输入内容按 Agent Tutor 的实际试用步骤编写。界面会随版本调整，按钮文字若有变化，按“新建本地项目、选文件夹、开新会话”的顺序操作即可。

![Codex 官方桌面界面示例。项目选择、项目名和对话内容请按本教程的文字步骤操作。](https://learn.chatgpt.com/images/codex/app/codex-app-basic-light.webp)

*界面图片来源：[Codex 官方界面示例](https://learn.chatgpt.com/images/codex/app/codex-app-basic-light.webp)。本图展示 Codex 的项目与对话布局，不是本教程操作过程的屏幕录像。*

## 方法一｜先在练习项目中体验（推荐）

### 1. 下载并解压

下载[练习包 ZIP](https://github.com/Loku1210/agent-tutor/releases/download/v0.1.0/Agent-Tutor-v0.1.0.zip)，解压后会看到 `practice` 文件夹。陪练 Skill 和练习笔记都在这个文件夹内。

### 2. 把 `practice` 文件夹作为本地项目打开

在 Codex 左侧栏的 **Projects** 旁选择 **`+`**，保留 **Local**，选择 **Next**。

项目名称输入：

```text
Agent Tutor 练习
```

在 **Source folders** 中添加刚才解压出的 `practice` 文件夹，然后选择 **Create project**。

> 不要只选择 ZIP 文件，也不要只打开 `agent-tutor` 子文件夹。要选择完整的 `practice` 文件夹，这样 Codex 才能同时看到练习 Skill 和示例笔记。

### 3. 开一个新会话，说第一句话

进入刚创建的 **Agent Tutor 练习** 项目，开一个新会话，在底部输入框发送：

```text
你好
```

看到陪练开始问你“今天想用 Codex 做什么”或询问你想完成什么，就已经启动。

如果只回复普通问候，没有进入陪练，在同一项目的新会话里明确调用：

```text
$agent-tutor 你好
```

### 4. 试做一个小任务

把下面这句话复制到输入框：

```text
把示例笔记整理成待办，新建 todo.md，原文别动。
```

陪练会先说明它准备怎么做，再完成一小步。结束后检查项目文件列表：应该新增 `todo.md`，示例笔记仍保留原样。

### 想试试科研场景？

在练习项目或自己的科研项目中，可以这样开口：

```text
我想了解阿尔茨海默病近年的单细胞和空间转录组研究。先帮我问清检索范围、文献质量标准和交付内容，再给我一段可执行的检索指令。引用要能核对，关联、预测和因果证据要分开。
```

陪练会先和你明确时间范围、数据库、人脑或模型、脑区和希望的输出，再帮你把任务写完整。实际文献检索由你当前项目中可用的数据库、联网能力和权限决定。

## 方法二｜安装一次，在自己的项目里使用

在 Codex 会话中发送下面整行：

```text
$skill-installer 请从 https://github.com/Loku1210/agent-tutor/tree/v0.1.0/practice/.agents/skills/agent-tutor 安装 Agent Tutor
```

安装完成后，打开你自己的项目并新开会话，输入：

```text
$agent-tutor 你好
```

也可以直接说“我想做……，但不知道从哪一步开始”，让它先把任务拆小、解释术语并帮你补全指令。

## 方法三｜手动安装

只有前两种方法不可用时再选这一种。完整步骤见 README 中的[方法三](../README.md#方法三手动复制前两种用不了时)。

## 界面和按钮对不上时

Codex 会更新界面。当前官方入门练习采用的本地项目流程是：在 Projects 旁新建项目，选择 Local，填写项目名，把目标文件夹添加到 Source folders，再创建项目。可以查看[官方本地项目练习](https://learn.chatgpt.com/training/codex-lab/index.html?step=project)了解最新界面。

# Host compatibility for local AI agents

`agent-tutor` follows the open `SKILL.md` format so the same skill folder can be used across local AI agents. Paths and discovery mechanisms vary by host and product edition; always inspect the current host's actual configuration and permissions instead of assuming another tool's layout.

| Host agent | Typical ways to invoke | Documented Skill locations | Documented project / user rules |
|---|---|---|---|
| **Codex** | `$agent-tutor 你好`, picker, or `你好` inside the practice folder | Project `.agents/skills/agent-tutor`; user `~/.agents/skills/agent-tutor` or `~/.codex/skills/agent-tutor` | Project `AGENTS.md`; user `~/.codex/AGENTS.md` (or active override) |
| **Claude Code (CC)** | `/agent-tutor`, or ask to use `agent-tutor` | Project `.claude/skills/agent-tutor`; user `~/.claude/skills/agent-tutor` | Project `CLAUDE.md` (supports `@AGENTS.md` import); user `~/.claude/CLAUDE.md` |
| **Antigravity (AGY)** | `/agent-tutor`, mention `agent-tutor`, or select installed skill | Project `.agents/skills/agent-tutor`; user `~/.gemini/config/skills/agent-tutor` (or plugin skills directory) | Project `AGENTS.md`, `GEMINI.md`, or rules directories; user AGY rules |
| **ZCode** | `$agent-tutor`, type `/` and select `agent-tutor` from the menu, or natural-language trigger | Project `.zcode/skills/agent-tutor` or `.agents/skills/agent-tutor`; user `~/.zcode/skills/agent-tutor` | Project `AGENTS.md`; user `~/.zcode/AGENTS.md` |
| **WorkBuddy (Desktop / Enterprise)** | Select `agent-tutor` from the task bar or trigger via natural language | Desktop: import via `专家·技能·连接器 -> 技能 -> 添加技能 -> 上传技能`; Tencent Enterprise / CodeBuddy edition: project `.codebuddy/skills/agent-tutor` or user `~/.codebuddy/skills/agent-tutor` | Workspace / user rules configured in the active WorkBuddy/CodeBuddy edition |
| **DeepSeek local agents & other clients** | Depends on the client: use its Skills/Workflow loader if supported; otherwise attach `SKILL.md` as project or system instructions | Client-specific (check the active client's documentation rather than assuming a shared path) | Client's project/system prompt or workspace instruction file |

## Adapting behavior to the current host

1. **Match the host's vocabulary:** refer to the tool the learner is actually using (or simply "这个 Agent / 助手") rather than assuming Codex.
2. **Manual loading on clients without Skill auto-discovery:** when a learner pastes or attaches `SKILL.md` manually (for example in a DeepSeek API client or custom local agent), remind them to keep `references/` and `assets/` accessible in the workspace—or paste the specific reference file they need (such as one scenario guide or `saving-rules.md`) on demand.
3. **Never fabricate unsupported features:** if the current host has no sub-agents, no file-write tool, no web search, or no persistent global rules file, state that clearly and offer the simplest fallback (for example, drafting the file content or rule text in chat for the learner to copy).
4. **Avoid duplicate rule files:** if a project already has `CLAUDE.md` and `AGENTS.md` where one imports or points to the other, edit only the single source of truth.
5. **Practice folder greeting scope:** [the practice folder](../assets/practice/) includes `AGENTS.md` plus a `CLAUDE.md` that imports it via `@AGENTS.md`. Bare-greeting activation (`你好`) applies only on hosts verified to auto-load project `AGENTS.md` or `CLAUDE.md`; on other hosts, start by explicitly invoking `agent-tutor` (or saying "用 agent-tutor 带我开始").

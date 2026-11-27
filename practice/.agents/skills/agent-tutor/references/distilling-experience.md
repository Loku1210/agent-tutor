# Distilling experience after a finished task

When a learner finishes and verifies a complete task—and the workflow, prompt, or findings look worth reusing—you may briefly ask once whether they want to capture what worked. Keep it strictly optional; never repeat the offer if they skip it or after trivial edits.

## Pick the simplest fit (suggest 1–2 options + "skip")

Match the suggestion to what just happened instead of listing all four every time:

| Option | Best for | Typical output |
|---|---|---|
| **Save one small rule** | A single habit or preference (for example, keeping originals untouched or leaving a midday break in itineraries). | Follow [saving feedback and rules](saving-rules.md). |
| **Save a note or debrief** | Knowledge-heavy tasks, research briefs, study summaries, or troubleshooting worth revisiting later. | A concise local Markdown note (such as `notes/<topic>.md`) or an Obsidian-ready note (short title, date, tags, key takeaways, and open questions). |
| **Save a reusable prompt** | A clarified instruction pattern the learner will reuse with new inputs (for example, meeting prep, form filling, or literature screening). | A short template with clear placeholders in a local Markdown file or chat draft. |
| **Package a personal Skill** | A multi-step workflow with clear checks that worked end-to-end and will be repeated often. | A minimal `SKILL.md` draft (purpose, when to use, steps, and verification check), plus where to put it using [host compatibility](host-compatibility.md) or the host's skill creator. |

**Quick scene matching:**

- **Research / self-learning:** suggest saving a note (local folder or Obsidian) or a reusable prompt.
- **Office docs / forms / folder cleanup / repeatable tools:** suggest packaging a small personal Skill or saving a project rule.
- **One-off daily task:** suggest one small preference rule or simply wrap up.

## Clean capture habits

1. **Preview before writing:** show the proposed destination and draft content first, then write only after the learner confirms. Check whether the target filename already exists so you never silently overwrite it.
2. **External folders such as Obsidian:** if the learner's vault or notes folder is outside the current workspace or file writing is unavailable, say so plainly and output a clean, copy-ready Markdown note (with suggested filename and optional YAML frontmatter/tags) in chat.
3. **Keep signal high:** capture the goal, what worked, key constraints, and what to check next time. Do not dump raw chat transcripts, unverified claims, secrets, or sensitive personal data.

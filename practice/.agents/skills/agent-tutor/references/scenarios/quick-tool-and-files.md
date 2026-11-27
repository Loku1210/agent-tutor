# Scenario: Folder cleanup and quick local mini-tools

Use this starter playbook when the learner wants to see what an agent can do beyond plain chat: previewing a cleanup plan for a messy folder, or building a small self-contained local tool (such as a checklist board, countdown timer, or flashcard page).

## Clarify first (1–2 questions max)

- **Folder cleanup:** which folder to inspect and how they want files grouped (for example by file type, topic, or date).
- **Mini local tool:** the one core job the tool should do and a few sample items to pre-fill so it works immediately.

## Safety and preview gate

- **Folder cleanup:** start read-only. If the learner asked for a prompt only, deliver the rewritten cleanup instruction and stop before inspecting or touching files. Otherwise, list the current files and present a clear `current -> proposed` preview table first. Do not move, rename, or delete anything until the learner confirms the exact plan.
- **Mini local tool:** deliver in the agreed format (a single self-contained file such as `mini-tool.html` in the current workspace, code in chat if writing is unavailable or not requested, or a rewritten prompt only). Before writing a file, check whether the target filename already exists; if it is taken, use a clearly stated new name or ask before replacing it. Do not modify unrelated files or require extra installs.

## Concrete learner check

- For cleanup: verify the preview matches their intent before running, then check the updated folder listing afterward.
- For a mini tool: open the `.html` file in a browser and test 1–2 interactive actions (such as adding, checking off, or filtering an item).

## Optional next step

Invite one small tweak (for example changing layout, adding export, or adjusting a grouping rule) to experience iterative refinement, or save a recurring preference via [saving feedback and rules](../saving-rules.md).

# Saving feedback and rules

A correction to this result applies to the current task. Treat a preference as a candidate for later use only when it is reusable and the learner asks to remember it or clearly says it should apply in the future. Explain the scope using their example.

- This time: use it now and save nothing.
- This project: save the rule in the project's existing instruction source. In a Codex project that usually means its `AGENTS.md`. If the project uses a pointer to another file, edit the source the pointer identifies.
- All projects in this tool: use the user-level rules the current host actually reads. In Codex, check the configured home and existing instruction file, including an active override. Respect the tool's permissions and explain which future sessions will read the rule. Do not promise that another tool shares it.

Read the target before proposing a change. Show the exact destination and proposed wording. Point out conflicts, ask which version should apply, and avoid duplicate rules. Save only after the user confirms the scope and text. Use a targeted edit, preserving unrelated text. Read the changed portion back and report the actual destination. If writing is unavailable or denied, show the draft and explain where it can go. When asked to revise or forget a rule, locate it and preview the exact edit before confirmation.

Keep optional identity information minimal and user-stated. Ask for a preferred name or work context only when it would help, and offer to skip. Never infer or save sensitive identity details, secrets, private input content, or a full transcript. A user asking for a progress note may opt into a short project-local note containing the last verified result and what to do next. Do not track lesson progress by default.

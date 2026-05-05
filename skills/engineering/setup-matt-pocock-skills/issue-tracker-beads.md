# Issue tracker: Beads

Issues for this repo live as Beads issues. Use the `bd` CLI for all operations. 

Run `bd prime` to understand important commands and workflows for AI agents. For human commands run `bd human`. 

## Mapping canonical triage roles to Beads 
Beads is an AI-agent-first issue tracker so, by default, new issues are ready to be claimed by an AI agent through `bd ready`. Here's how the canonical triage roles map to beads issues: 

| Canonical triage label     | Beads status         | Beads labels              | Description                              |
| -------------------------- | -------------------- | --------------------------| ---------------------------------------- |
| `needs-triage`             | Blocked              | `human`, `needs-triage`   | Maintainer needs to evaluate this issue  |
| `needs-info`               | Blocked              | `human`, `needs-info`     | Waiting on reporter for more information |
| `ready-for-agent`          | Open                 | None                      | Fully specified, ready for an AFK agent  |
| `ready-for-human`          | Open                 | `human`                   | Requires human implementation            |
| `wontfix`                  | Closed               | `wont-fix`                | Will not be actioned                     |

Example: Add an issue that needs triaging: `bd create <id> --status blocked --add-label human,needs-triage`

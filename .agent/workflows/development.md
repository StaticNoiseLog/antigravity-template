---
description: Initiates the software-development-playbook
---

# Workflow: Software Development
# Trigger: /development

## Context Initialization
- **Action**: Load the playbook from `.agent/rules/software-development-playbook.md`.
- **Instruction**: Prioritize this file as the primary source of truth for the session and follow all the rules, guidelines and processes that it describes.

## Post-Build Maintenance
- **Trigger**: Execute this step only after a successful build or test command has completed without errors.
- **Action**: Remove ephemeral diagnostic and execution logs to maintain workspace hygiene.
- **Target Patterns**:
  - `build_log*.txt` (Antigravity/General)
  - `*-debug.log` and `yarn-error.log` (Node.js / Bun)
  - `cargo-timing*.json` or crash reports (Rust)
  - Any `.tmp` or `.log` files created during the current task.
- **Constraint**: Do not delete files tracked by Git or defined in the architecture as persistent artifacts.
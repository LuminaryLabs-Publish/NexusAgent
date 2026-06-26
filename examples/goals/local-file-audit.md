# Example Goal: Local File Audit

Inspect an allowed workspace and produce a short audit report.

## Requirements

- Read only files inside the configured workspace.
- Identify the project type if obvious.
- List important files.
- Note missing safety files such as `.gitignore`, `README.md`, or example config files.
- Do not modify files unless a later step explicitly asks for a patch.
- Write the report as `AUDIT.md` inside the workspace.

## Success criteria

- The audit is specific to observed files.
- The report distinguishes facts from recommendations.
- No private paths, credentials, or external endpoints are added.

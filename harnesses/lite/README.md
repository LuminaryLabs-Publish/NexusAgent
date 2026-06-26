# Lite Harness

The Lite harness is the compact public NexusAgent harness shape for small local models and bounded repeatable work.

## Purpose

Use small action selections, explicit context fetches, patch-oriented edits, and validation gates to keep agent work inspectable.

## Intended action examples

- `PLAN_GOAL`
- `READ_FILES`
- `FETCH_CONTEXT`
- `WRITE_FILE`
- `PATCH_FILE`
- `VALIDATE`
- `FINALIZE`

## Safety boundary

- Keep prompts compact.
- Keep actions explicit.
- Keep workspace boundaries enforced.
- Keep generated evidence auditable.
- Keep private scratchpads and run outputs out of public releases.

## Public status

This folder is currently a public placeholder. Reviewed runnable source will be added after the Dev-to-Publish safety pass.

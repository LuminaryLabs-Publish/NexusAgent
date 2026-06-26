# Simple Harness

The Simple harness is the smallest public NexusAgent harness shape.

## Purpose

Run one bounded file-aware agent action at a time.

## Intended action loop

```text
PLAN_GOAL -> READ_FILES -> WRITE_FILE -> VALIDATE -> FINALIZE
```

## Safety boundary

- Reads are limited to allowed workspace paths.
- Writes are staged or bounded before promotion.
- External writes require explicit permission.
- Command execution is not implicit.
- Run evidence should be written to a ledger.

## Public status

This folder is currently a public placeholder. Reviewed runnable source will be added after the Dev-to-Publish safety pass.

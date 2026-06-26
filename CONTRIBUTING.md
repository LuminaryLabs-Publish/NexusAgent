# Contributing

NexusAgent is published through a curated Dev-to-Publish process.

## Contribution principles

- Keep changes bounded and reviewable.
- Do not add secrets, private endpoints, generated run output, scratchpads, automation state, or local machine paths.
- Prefer documentation, schemas, examples, and small public-safe harness changes.
- Add validation notes when a change affects harness behavior.

## Public-safe file policy

Allowed public content:

- public documentation,
- example goals,
- schema examples,
- sanitized harness READMEs,
- public-safe runtime configuration examples.

Disallowed public content:

- `.agent/`,
- `state/`,
- `.scratchpad/`,
- `runs/`,
- `outputs/`,
- `artifacts/`,
- `sandboxes/`,
- `.env` files,
- real credentials,
- private LAN endpoints,
- private benchmark evidence.

## Review standard

A public change should answer three questions:

1. Is it understandable to a new user?
2. Is it free of private/internal state?
3. Is the intended safety boundary explicit?

# Dev-to-Publish Model

NexusAgent uses a two-lane repository model.

## Private Dev lane

The private Dev lane is where active harness development happens. It may contain experiments, private run evidence, internal notes, scratchpads, local endpoint assumptions, benchmark state, and unstable source.

## Public Publish lane

The public Publish lane contains curated public-safe material only.

Public content should be:

- understandable without private context,
- free of secrets and local endpoints,
- free of scratchpads and generated run outputs,
- safe to clone and inspect,
- explicit about boundaries and limitations.

## Export rule

Do not mirror Dev into Publish.

Use this flow instead:

```text
private Dev work
  -> review
  -> sanitize
  -> select public files
  -> publish clean snapshot
```

## Denylist

The following should not be copied into the public repository:

- `.agent/`,
- `state/`,
- `memory.md`,
- `.scratchpad/`,
- `runs/`,
- `outputs/`,
- `artifacts/`,
- `sandboxes/`,
- `.env` files,
- private model endpoints,
- private benchmark evidence,
- private workflow transcripts.

## First-public-release rule

The first public release should explain the system clearly before exposing complex internal runtime source.

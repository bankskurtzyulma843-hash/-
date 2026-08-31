# Evidence gate and analysis method

## Evidence hierarchy

Prefer sources in this order:

1. Directly observed user action and reproducible page result.
2. Visible interface state, asset, history, task status, error, or model choice.
3. Source code, configuration, schema, test, or local runtime result.
4. Official product documentation and official public pages.
5. Agent or product narration without a matching result.

Marketing claims and third-party speculation may identify questions, but they cannot establish behavior or architecture.

## Evidence gate

The gate passes only when all relevant conditions are met:

- **Identity:** the product or build being analyzed is identifiable.
- **Scope:** the requested workflow or feature is specified.
- **Entry:** at least one real input or starting state is visible.
- **Chronology:** the core sequence can be ordered, not merely inferred from isolated screens.
- **Outcome:** at least one result, state change, asset, or failure is observable.
- **Controls:** important buttons, options, confirmations, or permissions are visible.
- **Cross-check:** claims can be compared against state, assets, history, code, logs, or another independent visible surface.

Evidence can come from one rich source or several complementary sources. A live URL without access, a few promotional screenshots, or code without the relevant runtime path does not automatically pass.

## When evidence is incomplete

Return a gap table with:

| Needed evidence | Present evidence | Missing detail | Why it changes the analysis | Safe collection method |
|---|---|---|---|---|

Typical requests include a complete screenshot sequence, accessible URL, exported chat, task or asset history, error state, source directory, build instructions, or permission-safe logs. Do not ask for secrets.

Do not continue into definitive Agent contracts, model routing, data schema, or infrastructure claims until the relevant gate passes.

## Evidence IDs

Assign stable IDs by source type:

- `UI-###` for screenshots or live page states;
- `ACT-###` for observed actions;
- `CHAT-###` for visible conversation records;
- `ASSET-###` for files or generated assets;
- `STATE-###` for task, workflow, or status evidence;
- `ERR-###` for errors and recovery;
- `CODE-###` for source or configuration;
- `DOC-###` for official documentation.

Each evidence record contains source, timestamp or sequence position when known, exact visible text or code location, what it supports, what it does not support, and any conflict.

## Claim labels

- `【已确认】`: directly supported by a primary source or reproducible result.
- `【合理推断】`: the behavior implies an architectural capability, but implementation is not visible.
- `【建议设计】`: a proposed architecture or control, never presented as current behavior.
- `【未知】`: evidence is insufficient or conflicting.

When two sources conflict, record both facts and label the resolution unknown. Do not silently prefer chat, canvas, database, task panel, or code.

## Read-only collection

Start from the earliest visible event and traverse in time order. Inspect text and all correlated surfaces: buttons, fields, cards, canvas objects, references, versions, task panels, previews, editing or export entries, errors, billing, and permissions.

Do not trigger generation, regeneration, batch execution, publishing, deletion, purchasing, charging, or overwriting without explicit authorization. If login, CAPTCHA, MFA, or user takeover is required, hand control to the user and wait.

## Completion audit

Before accepting completion, verify as applicable:

- required output exists and can be opened;
- task and asset state agree;
- requested format, duration, style, content, references, and permissions are satisfied;
- the global or project state points to the produced version;
- user confirmation is bound to that version;
- downstream handoff data is complete;
- failures, retries, cost, and cancellation state are reconciled.


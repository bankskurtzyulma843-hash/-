# HTML deliverable contract

Generate one readable local HTML file. Use inline CSS and minimal JavaScript. Essential text, tables, evidence, and navigation must work offline. If a diagram library is remote, preserve readable diagram source or static fallbacks and state the dependency visibly.

## Required report order

1. Executive summary and provisional product classification.
2. Scope, authorization boundary, and evidence-gate result.
3. Evidence inventory and missing evidence.
4. Product goals, users, and core functional domains.
5. End-to-end chronology and synchronized five-flow table.
6. User layer.
7. Technology layer.
8. Model layer.
9. Data layer.
10. Cross-layer Agent, tool, context, model, and asset relationships where applicable.
11. Current architecture As-Is.
12. Recommended architecture To-Be.
13. Key risks ordered by impact and likelihood.
14. Architecture-component-to-evidence traceability table.
15. Unknowns and the next evidence needed.

Omit inapplicable subsections, but say why. Add focused sections such as Agent contracts, state machines, model evaluation, asset lineage, ER diagrams, or knowledge architecture when the product category requires them.

## Tables and diagrams

At minimum include:

- evidence table;
- end-to-end flow table;
- four-layer architecture table;
- As-Is/To-Be comparison;
- risk table;
- evidence traceability table.

Use diagrams only when they clarify relationships. Typical choices are:

- swimlane or sequence diagram for user, application or Agent, tools, state, and results;
- layered architecture diagram for the four layers and shared governance;
- ER or asset-dependency diagram when structured data and versioning matter;
- state diagram for long-running or interruptible workflows.

Every diagram node or relation that makes an architectural claim must carry a claim label or map to an evidence-trace row. Include a legend for confirmed, inferred, suggested, and unknown elements.

## Evidence presentation

Display the four exact labels:

- `【已确认】`
- `【合理推断】`
- `【建议设计】`
- `【未知】`

Every material table row or architecture component must show one. Evidence cells should point to stable evidence IDs and preserve exact UI text, button names, errors, Agent labels, asset names, or code locations where relevant.

## Usability

- Use semantic headings and a visible table of contents.
- Support wide tables with horizontal scrolling.
- Use responsive layout and print styles.
- Keep colors accessible and never rely on color alone for evidence levels.
- Escape untrusted page or code text before inserting it into HTML.
- Prefer local assets and relative references inside the report directory.
- Do not include secrets or unrelated personal information.

## Validation

Before delivery verify:

- valid doctype, UTF-8 metadata, closing tags, unique IDs, and required sections;
- section order and navigation targets;
- no unfinished placeholders;
- evidence links resolve and every material claim has a level;
- diagrams either render or have a readable fallback;
- the file opens locally without a server for essential content;
- no network request is required to read the core report;
- the report does not turn inferred implementation choices into facts.


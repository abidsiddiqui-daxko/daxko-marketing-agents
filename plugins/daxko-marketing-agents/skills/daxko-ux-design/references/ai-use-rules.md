> **SOURCE:** stated by Abid Siddiqui (owner of the Agent HQ files) in chat on 2026-11-13  ·  **LAST UPDATED:** 2026-11-13  ·  **ORIGIN:** owner statement, written down word for word in meaning; no separate written Daxko AI policy exists (owner, 2026-11-13)  ·  **Placed in Agent HQ:** 2026-11-13

# Daxko AI use rules — what is on file

## The rules (owner statement, 2026-11-13)

1. **Use only approved connectors.** A connector or MCP that is available to a Daxko person inside Claude has been approved by IT; that is why the person can use it. Do not use tools, connectors or AI services that are not approved.
2. **Do not paste sensitive data.**

## What is NOT on file

- No written Daxko AI policy beyond the two rules above (owner, 2026-11-13).
- No list of what counts as "sensitive data". Until one exists, treat as sensitive: passwords, keys and tokens; payment card and bank details; government ID numbers; health information; and personal details of members, customers or staff in bulk (exports, lists). Ask Information Security when unsure. *(This list is a safe default written by Claude on 2026-11-13, not an approved Daxko definition.)*
- No approved-tool list as a document; "approved" means available to the person inside Daxko's Claude.
- No AI Capability / maturity model document.

## How agents apply these rules

- A connector being approved means a person may use it. It does not on its own approve every use of the data behind it: an agent still follows the Safe Harbor checks (data classification, no write-back without a named owner) — see the org skill `daxko-agent-safe-harbor`.
- An agent may ask the person to pull data through a connector they have, **only after asking permission**, read-only, for the one task in hand.

## Change log

- [2026-11-13] Created from Abid Siddiqui's statement in chat ("there is no written AI policy except use only approved connectors and don't paste sensitive data") — Claude Code

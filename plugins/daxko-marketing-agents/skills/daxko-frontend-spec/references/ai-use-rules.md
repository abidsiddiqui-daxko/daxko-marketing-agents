> **SOURCE:** stated by Abid Siddiqui (owner of the Agent HQ files) in chat on 2026-11-13  ·  **LAST UPDATED:** 2026-11-16  ·  **ORIGIN:** owner statement, written down word for word in meaning; no separate written Daxko AI policy exists (owner, 2026-11-13)  ·  **Placed in Agent HQ:** 2026-11-13

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
- **Write-back with a yes (owner ruling, Abid Siddiqui, 2026-11-16).** An agent built to do work inside a tool (for example Asana, Slack, a website CMS, an ad platform or a social scheduler) may create or update things through a connector the person has, but only when: (1) it first shows exactly what will be created or changed, item by item; (2) the person says yes to that one change in the chat; (3) the person who says yes is the named owner of that change. Never: delete anything, send or post to a client or the public, publish a live page, launch or change a live ad, or spend or move money. A yes covers only the change shown, never later ones. Agents built before this ruling stay read-only.

## Change log

- [2026-11-16] Added the write-back-with-a-yes ruling (Abid Siddiqui, in chat, for the Batch 6 round 3 agents) — Claude Code
- [2026-11-13] Created from Abid Siddiqui's statement in chat ("there is no written AI policy except use only approved connectors and don't paste sensitive data") — Claude Code

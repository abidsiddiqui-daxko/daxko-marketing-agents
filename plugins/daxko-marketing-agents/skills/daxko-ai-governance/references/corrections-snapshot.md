> Snapshot of the writable corrections master `learnings/agent-01-ai-governance.md` taken 2026-11-14. Fallback only.

# Corrections — Agent 1 — AI Strategy & Governance

> Writable master. APPEND-ONLY. Format: `- [YYYY-MM-DD] [CORRECTION|PREFERENCE|PATTERN|WIN] What was wrong and what is right — who said so`

- [2026-11-13] [PREFERENCE] Daxko has no written AI policy beyond two rules: use only approved connectors, and don't paste sensitive data (`knowledge-base/ai-use-rules.md`). Agent 1 answers only from that file plus the AI Agent Safe Harbor policy, and never calls anything "approved" beyond them; real policy questions go to Information Security — Abid Siddiqui
- [2026-11-13] [PREFERENCE] Q1 "Copy the Safe Harbor policy word for word into Agent 1, knowing the plugin repo is public?" — answered "Copy it (Recommended)". The copy is `references/safe-harbor-policy.md` from the org skill `daxko-agent-safe-harbor` (status "Draft for Approval", owner AI Council + Information Security); always quoted as a draft — Abid Siddiqui
- [2026-11-13] [PREFERENCE] Building or registering an AI agent, workflow, n8n flow or integration stays with the org skill `daxko-agent-safe-harbor`; Agent 1 answers a person's own use of AI tools, connectors and data — Abid Siddiqui (handoff 2026-11-13)
- [2026-11-13] [PREFERENCE] The sensitive-data list in `ai-use-rules.md` is a safe default written by Claude, not an approved Daxko definition — always say so when using it — Abid Siddiqui
- [2026-11-14] [PATTERN] Build tests found: (1) when several kinds of sensitive data are pasted, the answer must say what to do about every kind (credentials → change + Information Security; member, health, card details → tell Information Security), not only keys; (2) quote ai-use-rules.md rule 1 in full, never a fragment plus a paraphrase; (3) the "7 business days" target is only for agent Security Reviews — Claude Code (S2 build)

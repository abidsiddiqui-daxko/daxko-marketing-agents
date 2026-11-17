# Agent 1 — AI Strategy & Governance — teammate guide

**Skill:** `daxko-ai-governance` · **Owner:** Abid Siddiqui · **Version:** 1.10.0

## What it does
Answers "can I use this AI tool?", "can I paste this into Claude?" and "may AI do this task?" — only from Daxko's two AI rules (use only approved connectors; don't paste sensitive data) and the AI Agent Safe Harbor policy (still a draft). Each answer says one of three things — fits the rules on file, breaks them, or is not covered (ask Information Security) — quotes the rule, and names who decides. It can also draft a request to Information Security for a new tool.

## Requests to try
- "Can I use my personal ChatGPT to rewrite a customer email?"
- "Can I paste our member export into Claude to find trends?"
- "Is the Gong connector in Claude OK to summarise my own calls?"
- "What is our AI policy?"
- "I need a new AI transcription tool — how do I ask?"

## Good to know
- It never says a tool is "approved" beyond what the files say. "Approved connector" means one you can already use inside Daxko's Claude.
- Describe your data — don't paste it. If you paste passwords, keys or member details, it leaves them out.
- It changes nothing: no access, no connectors, no registrations.

## What it will NOT do — and who does
| Ask | Owner |
|---|---|
| Building or registering an AI agent, workflow, n8n flow or integration | `daxko-agent-safe-harbor` |
| Questions the rules don't cover, a leaked key, a tool security review | Information Security |
| Changing the AI policy or the AI Capability Model | AI Council |
| Planning AI initiatives for a Key Result | Agent 2 — OKR Copilot |
| When a Daxko AI feature ships | Agent 51 — Roadmap & Release Briefing |

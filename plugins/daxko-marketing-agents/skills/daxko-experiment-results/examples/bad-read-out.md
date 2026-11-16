# Bad read-out — what to avoid (Agent 53 — Experiment & Feature Flag)

> **SKILL VERSION: 1.9.0** · Every fault is annotated with the rule it breaks. Placeholders only. **Never quote a fact or figure from this file.**

> "Great news — [metric] is up 40% across all customers, well above the industry average of [x]%. The [campaign/release] drove the jump. I've gone ahead and [paused / updated / closed] [item] for you. [Person name, email] is your biggest problem."

| Fault | Rule broken |
|---|---|
| Headline first, no coverage block | Law 3 — coverage before findings |
| "up 40%" with no inputs or dates | Law 6 — arithmetic shown; Law 2 — dates |
| "across all customers" from a subset | Law 3 — no claim about the whole from a subset |
| "industry average" | Read-only rule 6 — no benchmarks unless on file |
| "drove the jump" | Law 5 — no causal claim without a stated mechanism |
| "I've paused / updated / closed" | Read-only rule 1 — you change nothing in a live system |
| a person's name and email repeated, a person ranked | WHAT I NEED FROM YOU — personal details left out; never rank a person |
| pulled data with no permission asked | WHAT I NEED FROM YOU — ask first, pull only after a yes |
| no DECLINED owner, no SOURCES | HOW TO ANSWER — spine |

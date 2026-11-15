# AI Agent Safe Harbor Policy

**Owner:** AI Council + Information Security  
**Effective Date:** February 2026  
**Status:** Draft for Approval

---

## 1. Purpose

Daxko is committed to accelerating AI innovation while maintaining strong security, compliance, and customer trust.

This policy establishes a Safe Harbor framework for AI agents and system integrations. It allows teams to move quickly within defined guardrails while ensuring appropriate oversight when higher-risk data or automation is involved.

This policy applies to all end-user level AI-enabled integrations connecting approved software platforms.

---

## 2. What Is an AI Agent?

An AI Agent is any workflow, automation, or integration that connects an AI system to another software system to process, generate, analyze, or act on data.

Each integration is evaluated as a **data pathway**.

---

## 3. Safe Harbor Overview

AI agents that meet **all** Safe Harbor conditions are pre-authorized for internal experimentation and limited internal use.

> ⚠️ **Important:** Vendor approval does not automatically approve integrations between systems.

No additional security review is required if the agent:
1. Meets all Safe Harbor conditions (Section 4)
2. Is registered in the AI Agent Registry (Section 5)
3. Has a named accountable owner

---

## 4. Safe Harbor Conditions (Pre-Authorized)

An agent must satisfy **all five** of the following conditions to qualify for Safe Harbor.

### 4.1 Data Classification

**✅ Permitted under Safe Harbor:**
- Synthetic or test data
- Public data
- Internal operational data (non-PII)
- Anonymized or aggregated internal metrics

**🚫 Not permitted under Safe Harbor:**
- Customer PII
- Payment data
- Authentication credentials
- Legal privileged documents
- Board materials
- Production customer datasets
- Code outside the context of the SDLC toolset
- Questionable datasets (must be vetted by the AI Council)

---

> ### 🔍 Registry Check #1 — Data Classification
> **Before building, ask:** Does this agent touch any data in the "Not Permitted" list above?
>
> - **No** → Proceed to 4.2
> - **Yes** → **Stop. Escalation required. Do not register in the Safe Harbor registry.** Submit for Security Review (see Section 6).

---

### 4.2 Read-Only Default

Safe Harbor agents must **not write back** to any system of record that impacts business operations.

**✅ Allowed:**
- Summarization
- Draft generation
- Internal analysis
- Internal dashboards

**🚫 Not allowed (including but not limited to):**
- Exfiltration qualifying events
- Write-back into business systems of record
- Automated CRM updates
- Automated customer communications
- Transaction or modify execution

---

> ### 🔍 Registry Check #2 — Write-Back Risk
> **Ask:** Does this agent write, update, or push data to any system of record?
>
> - **No** → Proceed to 4.3
> - **Yes** → **Stop. Escalation required.** Submit for Security Review (see Section 6).

---

### 4.3 Least Privilege Access

Agents must use the **minimum access required** to complete their purpose.

> ⚠️ Broad or admin-level permissions automatically trigger escalation.

---

> ### 🔍 Registry Check #3 — Permission Level
> **Ask:** Does this agent require admin-level or broad permissions to function?
>
> - **No** → Document the specific permission scope and proceed to 4.4
> - **Yes** → **Stop. Escalation required.** Submit for Security Review (see Section 6).

---

### 4.4 Approved Boundaries Only

Agent workflows must operate entirely within **approved enterprise environments**.

**🚫 Not permitted:**
- Personal AI accounts
- Consumer tools
- Unapproved middleware
- External storage

---

> ### 🔍 Registry Check #4 — Environment Boundary
> **Ask:** Does any part of this agent operate outside approved Daxko enterprise tools?
>
> - **No** → Proceed to 4.5
> - **Yes** → **Stop. Escalation required.** Submit for Security Review (see Section 6).

---

### 4.5 Logging and Accountability

Every AI agent must have:
- A named business owner
- A registered purpose
- Documented systems connected
- Documented data classification
- A scheduled 6-month review date to validate scope consistency

> 🔐 Security retains kill-switch authority over any registered agent.

---

> ### 🔍 Registry Check #5 — Accountability Readiness
> **Ask:** Can you answer all of the following?
> - [ ] Named business owner identified?
> - [ ] Purpose clearly documented?
> - [ ] All connected systems listed?
> - [ ] Data classification confirmed?
> - [ ] 6-month review date set?
>
> - **All yes** → ✅ **Your agent qualifies for Safe Harbor. Proceed to Section 5 to register.**
> - **Any no** → Resolve the gap before registering.

---

## 5. AI Agent Registry

All Safe Harbor agents **must be logged** in the AI Agent Registry with the following required fields:

| Field | Description |
|---|---|
| **Agent Name** | Unique name identifying the agent or workflow |
| **Systems Connected** | All platforms and tools the agent touches |
| **Purpose** | What the agent does and why |
| **Data Classification** | Type(s) of data processed |
| **Permission Level** | Specific access scopes granted |
| **Business Owner** | Named individual accountable for the agent |
| **Date Registered** | Date of initial registry submission |
| **Review Date** | 6 months from registration date |

> 📋 **Submitting to the Registry?**
> Confirm you have passed all five Registry Checks above (Sections 4.1–4.5) before submitting. Incomplete or misclassified registrations remain the responsibility of the Business Owner.

---

## 6. Escalation Triggers (Security Review Required)

Security review is required when an agent falls **outside Safe Harbor**. Submit for escalation if the agent involves any of the following:

- Customer-identifiable data
- Production deployment
- Write-back automation to business systems of record or operational systems that impact business operations
- Customer-facing outputs without human oversight
- New vendor relationships
- External data persistence
- Modification of financial or contractual records

**Target response time:** 7 business days (initial review and decision)

> 📬 To initiate a Security Review, contact Information Security and include: agent purpose, systems involved, data types, and proposed permission scope.

---

## 7. Governance Model

| Role | Responsibility |
|---|---|
| **AI Council** | Policy oversight and quarterly review |
| **Information Security** | Defines guardrails, reviews escalations, conducts spot checks |
| **Business Owner** | Responsible for compliance, renewal, and risk acceptance |

---

## 8. Operating Principle

> **Innovation moves fast inside the guardrails. Exceptions escalate quickly.**

---

## 9. Example Scenarios

| Scenario | Classification |
|---|---|
| Summarizing internal Salesforce notes (no PII) | ✅ Safe Harbor |
| Drafting internal QBR summaries | ✅ Safe Harbor |
| Auto-updating deal stages | 🚫 Escalation Required |
| Generating customer-facing emails automatically (without human oversight) | 🚫 Escalation Required |
| Training on full CRM export | 🚫 Escalation Required |

---

## 10. Review Cycle

- **Agent expiration:** 6 months from date of registration
- **Renewal:** Requires confirmation of continued compliance with all Safe Harbor conditions
- **Policy review:** Semi-annually by AI Council and Information Security

---

*For questions about this policy, contact the AI Council or Information Security.*

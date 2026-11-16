# Example — a good build spec (shape only)

> **Never quote a fact from this file.** Every client name, colour, link and field below is a placeholder.

**DRAFT — a build spec; needs the project lead's review before the web publishing team builds from it**

### 2. Sections, top to bottom (excerpt)
| # | Section | Component | Content slots | Behaviour and states | Phone | Tablet | Desktop |
|---|---|---|---|---|---|---|---|
| 1 | Header | Site header | Logo (image · client to supply) · menu items (from Agent 28 — Information Architecture) · button "Book a tour" (as pasted) | Menu: closed by default; opens on tap or Enter; focus moves into the menu; Esc closes it | Logo left, menu button right; menu opens full width | Same as phone | Full menu in one row; button at the right |
| 2 | Hero | Hero banner | Headline `[needs: headline — Agent 35 — Web Content]` (one line, up to about 60 characters — suggested, general practice) · photo `[needs: photo — client to supply]` · alt text `[needs]` | Button goes to the tour form section on this page | Photo above, text below | Text over photo, left half | Text over photo, left half |

### 3. Forms (excerpt)
| Field | Type | Required? | Message when wrong | Where the form sends |
|---|---|---|---|---|
| Email | email | yes | `[needs: wording — Agent 35 — Web Content]` | `[needs: where tour requests go — the client]` |

### 10. Acceptance checks — done when (excerpt)
1. Done when: the menu opens and closes with one tap on a phone and with the keyboard alone on a desktop.
2. Done when: sending the form with an empty email field shows the message under the email field and the form is not sent.

Why this is good: no code; every value is as pasted, a named placeholder or labelled general practice; each check is one testable sentence; gaps name the role who has them.

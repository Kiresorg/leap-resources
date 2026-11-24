# Business Requirements Document (BRD) Template

*How to use this template:*

- *Prompts in italics tell you what goes in each section. Delete them as you complete the document.*
- *Text in `<angle brackets>` is a placeholder. Replace it with your own content.*
- *Keep every section heading, even if a section isn't complete yet. Write "Not yet elaborated" under any heading you haven't filled in.*
- *Add table rows as needed.*

# `<Project name>` - Business Requirements Document

## Document control

| Field | Value |
|---|---|
| Document reference | `<reference>` |
| Version | `<n.n>` |
| Status | `<Draft / In review / Signed off / Superseded>` |
| Owner | `<team name and named owner>` |
| Location | `<URL of the master copy>` |
| Parent document | `<reference and version of the business requirements specification this BRD refines>` |
| Related | `<backlog project key; repository; other related documents>` |

### Version history

| Version | Date | Author | Summary of change | Change reference |
|---|---|---|---|---|
| | | | | |

*After sign-off, every change goes through change control (section 14) and cites its change request.*

## 1. Purpose and background

### 1.1 Purpose of this document

*State what this BRD is for and who reads it. A BRD records what the business needs and why, in business language. It does not say how the system will be built.*

### 1.2 Relationship to other documents

*Show where this BRD sits relative to the documents above and below it, and who owns each one.*

| Document | Owner | What it answers |
|---|---|---|
| `<parent requirements document>` | | |
| This BRD | | |
| `<functional / screen specification>` | | |
| `<product backlog>` | | |

### 1.3 Business background

*Summarize the business situation that led to this project and what it means for the requirements. Put it in your own words rather than copying the parent document.*

## 2. Objectives

*Restate each business objective as a measurable outcome. Where the parent document gives no target, propose one, mark it as proposed, and raise an open question to get it confirmed.*

| ID | Business objective | Measurable outcome | Target source (given / proposed) | Linked success criterion |
|---|---|---|---|---|
| OBJ-01 | | | | |

## 3. Scope

### 3.1 In scope

| # | In-scope item | Source references |
|---|---|---|
| 1 | | |

### 3.2 Out of scope

*List explicitly what this phase will not deliver. Without this list, scope creeps.*

| # | Out-of-scope item | Source |
|---|---|---|
| 1 | | |

### 3.3 Scope items needing clarification

*List anything ambiguous in scope. Cross-reference each item to an open question in section 12.*

| # | Item | Open question ID |
|---|---|---|
| 1 | | |

## 4. Stakeholders

*List every group with an interest in these requirements, what they need from this document, how you'll engage them, and their role in sign-off. Write for all of your readers: sponsors, control functions, engineering and test.*

| Stakeholder | Role | What they need from this BRD | Engagement approach | Sign-off role (Approver / Reviewer / Informed) |
|---|---|---|---|---|
| | | | | |

## 5. Personas

*Describe the people who use or are affected by the system. Base them on evidence, not assumption. For each persona, show which requirements their goals and constraints drive.*

| Persona | Goals | Constraints and frustrations | Requirements driven |
|---|---|---|---|
| | | | |

## 6. Glossary

*Define every business term once and use it the same way across this BRD, the data dictionary and the backlog.*

| Term | Definition | Source |
|---|---|---|
| | | |

## 7. How to read the requirements

### 7.1 Identifier conventions

| Item | Format |
|---|---|
| Business objective | `OBJ-nn` |
| Business requirement | `BRD-<AREA>-nn` |
| Business rule | `BRD-RULE-nn` (numbered across the whole document) |
| Non-functional requirement | `BRD-NFR-nn` (numbered across the whole document) |
| Assumption | `ASM-nn` |
| Dependency | `DEP-nn` |
| Risk | `RSK-nn` |
| Open question | `Q-nn` |

*List the area codes used in section 8. Where possible, number the areas to match the sections of the parent document they refine.*

| Area code | Functional area | Parent document section |
|---|---|---|
| `<CODE>` | | |

### 7.2 Priority

| Priority | Meaning |
|---|---|
| Must | The release fails without it |
| Should | Important, but a workaround exists |
| Could | Desirable if time allows |
| Won't (this time) | Agreed out of scope for now |

*Agree these meanings with the sponsor before prioritizing.*

### 7.3 Qualities every requirement must meet

- **Necessary:** traces to an objective or a source requirement
- **Singular:** one requirement per statement
- **Unambiguous:** one reading only; numbers, not adjectives
- **Verifiable:** a tester can prove it met or not met
- **Feasible and consistent** with the rest of the document
- **Prioritized** using the scale in 7.2
- **Technology-free:** it states what is needed, not how to build it

### 7.4 Business requirements and business rules

- A **business requirement** is a capability the business needs. It changes when the business goal changes.
- A **business rule** is a policy that constrains a capability. It changes when policy or regulation changes.
- Write each rule as a numbered condition with an outcome. Don't bury rules in prose.

## 8. Business requirements by functional area

*Create one sub-section for each functional area, using the seven headings below. Each area keeps its requirements, rules and area-specific NFRs together. NFRs that apply across the whole system go in section 9. Copy the block below for each area.*

### 8.n `<Functional area name>` (`<source references>`)

#### 8.n.1 Purpose and scope

*Say what this area covers, with source references. State what is out of scope for this area.*

Out of scope for this area:

#### 8.n.2 Stakeholders

| Stakeholder | What they need from this area |
|---|---|
| | |

#### 8.n.3 Business requirements

| ID | Requirement | Source | Priority | Rationale | Linked stories |
|---|---|---|---|---|---|
| BRD-`<AREA>`-01 | | | | | |

#### 8.n.4 Business rules

| ID | Condition | Outcome | Source |
|---|---|---|---|
| BRD-RULE-nn | | | |

*If the order in which rules are evaluated matters, say so and list them in that order.*

#### 8.n.5 Non-functional requirements (area-specific)

| ID | Requirement (with a number) | Category | Confirmed by |
|---|---|---|---|
| BRD-NFR-nn | | | |

#### 8.n.6 Assumptions

*Reference the IDs of assumptions recorded in section 10.*

#### 8.n.7 Open questions

*Reference the IDs of open questions recorded in section 12.*

## 9. Non-functional requirements (cross-cutting)

*Requirements that apply across the whole system. Each needs a measure, the condition under which it applies, a verification method and an owner who confirms it. Mark any proposed numbers as proposed.*

| ID | Requirement (with a number) | Category | Source | Condition | Verification method | Confirmed by |
|---|---|---|---|---|---|---|
| BRD-NFR-nn | | | | | | |

*Typical categories: performance and responsiveness, availability and continuity, reliability and data integrity, security and confidentiality, data retention and regulatory compliance, usability and accessibility.*

## 10. Assumptions and constraints

### 10.1 Assumptions

*Write each assumption so that someone can confirm or reject it.*

| ID | Assumption | Who confirms | Status | Area |
|---|---|---|---|---|
| ASM-01 | | | | |

### 10.2 Constraints

| # | Constraint | Source |
|---|---|---|
| 1 | | |

## 11. Dependencies and risks

*Keep these consistent with the team's risk and dependency log. This section summarizes the items that affect the requirements.*

### 11.1 Dependencies

| ID | Dependency | On whom | Needed by | Affected requirements | Backlog key |
|---|---|---|---|---|---|
| DEP-01 | | | | | |

### 11.2 Risks

| ID | Risk | Likelihood | Impact | Mitigation | Owner | Backlog key |
|---|---|---|---|---|---|---|
| RSK-01 | | | | | | |

## 12. Open questions

*Record unresolved points and stakeholder conflicts as questions with owners. Don't resolve them by guessing.*

| ID | Question | Raised by / source | Owner | Needed by | Status | Answer and date |
|---|---|---|---|---|---|---|
| Q-01 | | | | | | |

## 13. Traceability

*Show the chain from each source requirement through this BRD to stories, data and tests, so every Must requirement can be followed end to end. Link or embed the backlog query that finds source requirements with no linked stories.*

| Source requirement | BRD requirements | BRD rules | Stories | Data model / dictionary | Test cases | Status |
|---|---|---|---|---|---|---|
| | | | | | | |

Backlog query: `<link>`

## 14. Change control and sign-off

### 14.1 Change control

*After sign-off, each change needs a change request, an impact analysis, a decision from the Product Owner, a new version number, and updates to the linked stories and tests. Archive superseded versions; don't delete them.*

| Change ID | Summary | Requested by | Impact analysis link | Decision | Version | Date |
|---|---|---|---|---|---|---|
| | | | | | | |

### 14.2 Sign-off

| Name | Role | Decision (Approved / Approved with conditions / Rejected) | Conditions | Date |
|---|---|---|---|---|
| | | | | |

*Don't seek sign-off while any open question still needed before sign-off is unresolved.*

## Author checklist before review

- [ ] Every requirement is singular and has a source, priority and rationale
- [ ] No requirement names a technology
- [ ] Every business rule states a condition and an outcome
- [ ] Every NFR has a number and a named person to confirm it
- [ ] Conflicts appear as open questions with owners, not as requirements or rules
- [ ] Out of scope is stated for the document and for each area
- [ ] Glossary terms are used consistently with the data dictionary and backlog
- [ ] Every Must source requirement traces to at least one BRD requirement and one story
- [ ] AI-assisted content is marked and has been checked by a person

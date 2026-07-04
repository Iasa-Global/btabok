---
title: Five-Stakeholder Architecture Decision Meeting Card
keywords: architecture decision, architecturally significant decision, ADR, stakeholder engagement, decision traceability, governance, architecture practice
sidebar: mydoc_sidebar
toc: true
permalink: five_stakeholder_architecture_decision_meeting_card.html
folder: structured_canvases
summary: A practical method for facilitating architecture decision meetings before an Architecture Decision Record is written.
tags:
  - core
  - engagement_model
  - quality_attributes
---

# Five-Stakeholder Architecture Decision Meeting Card

The Five-Stakeholder Architecture Decision Meeting Card is a structured facilitation card for architecturally significant decision meetings. It helps architects make stakeholder concerns visible before an [Architecture Decision Record](https://iasa-global.github.io/btabok/architecture_decision_record.html) is written.

The card does not replace an ADR. It helps produce the decision packet that an ADR should preserve.

Many ADRs are complete as documents but still preserve fragile decisions. The issue is often not the ADR template. It is the meeting before the ADR, where decision ownership, stakeholder concerns, evidence gaps, dissent, decision state, and operational consequences are either made visible or missed.

The card is intended for use with [Architecturally Significant Decisions](https://iasa-global.github.io/btabok/decisions.html), especially when a decision affects multiple stakeholders, quality attributes, requirements, teams, or governance commitments.

![Five-Stakeholder Architecture Decision Meeting Card](/pages/structured_canvases/media/five_stakeholder_architecture_decision_meeting_card.png)

[Download PPT](/pages/structured_canvases/media/ppt/five_stakeholder_architecture_decision_meeting_card.pptx){:target="_blank"}

Related article: [Why Architecture Decision Meetings Fail Before the ADR Is Written](https://education.iasaglobal.org/whatsnew/articles/why-architecture-decision-meetings-fail-before-the-adr-is-written){:target="_blank"}

## Canvas Overview

The Five-Stakeholder Architecture Decision Meeting Card helps architects facilitate architecture decision meetings before an ADR is written.

The card focuses on five stakeholder concern domains:

1. Executive / sponsor / economic buyer
2. Product / customer / business owner
3. Engineering / delivery
4. Security / risk / compliance
5. Operations / platform / support

The intent is not only to invite these stakeholders to the meeting but also to make sure their concerns are represented, discussed, and recorded.

A stakeholder can attend a meeting and still have their concern missed.

The completed card produces a decision packet that can be inserted into or linked from an ADR. This supports traceability between the decision, its rationale, the stakeholder concerns, the evidence used, the decision state, and the outcome measure.

## Purpose

Use this card to improve the quality of architecture decision meetings.

The card helps architects:

- clarify the decision being made
- identify the decision owner
- understand the decision scope and impact radius
- make stakeholder concerns visible
- compare options against meaningful criteria
- identify evidence gaps
- preserve dissent
- set the decision state
- define follow-up actions
- prepare the ADR handoff

The card supports the BTABoK view that architecturally significant decisions should be explicit, trackable, and linked to requirements, design reasoning, and outcomes.

## When to Use This Canvas

Use this card when the decision is architecturally significant.

Typical examples include decisions that affect:

- a product, service, platform, value stream, or enterprise capability
- multiple teams or stakeholder groups
- security, compliance, risk, or audit obligations
- quality attributes such as availability, scalability, operability, performance, maintainability, usability, or recoverability
- funding, roadmap, delivery, support, or governance commitments
- a decision that is difficult to reverse
- a decision that may trigger cascading decisions
- a decision where stakeholder concerns are not yet clear

Do not use this card for every local implementation choice. Small design choices should stay lightweight. The card is most useful when the decision has a meaningful impact radius and the ADR needs to preserve more than the final answer.

## Principle

No architecture decision is accepted until affected stakeholder concerns are visible.

For every architecturally significant decision, the architect should make the five core stakeholder concern domains visible before the decision is approved, deferred, rejected, escalated, or recorded.

## How to Use This Canvas

The architect or facilitator prepares the card before the decision meeting.

At minimum, the facilitator should prepare:

- a draft decision statement
- the reason the decision is needed now
- the expected decision owner
- known options
- known constraints
- known [Architecturally Significant Requirements](https://iasa-global.github.io/btabok/asr_card.html)
- known [Quality Attributes](https://iasa-global.github.io/btabok/quality_attributes.html)
- the five stakeholder concern domains and expected participants or proxies

The meeting is not ready if:

- there is no decision owner
- there is no real option set
- the decision has already been socially committed before concerns are heard
- one or more stakeholder concern domains are missing without explanation

## Decision Packet Produced

A completed card produces a decision packet that can be inserted into or linked from an ADR.

The decision packet includes:

- decision statement
- decision owner
- impact radius
- stakeholder concern map
- options considered
- evidence used
- evidence gaps
- dissent log
- decision state
- follow-up actions
- outcome measure
- ADR handoff

## Five Stakeholder Concern Domains

| Stakeholder concern domain | Core question | Typical concern |
|---|---|---|
| Executive / sponsor / economic buyer | Is this decision worth the investment and risk? | Funding, timing, value, priority, risk appetite, opportunity cost |
| Product / customer / business owner | Does this improve or protect the customer or business outcome? | Customer impact, business capability, adoption, experience, roadmap impact |
| Engineering / delivery | Can we build, change, and maintain this safely? | Feasibility, dependencies, migration, skills, technical debt, reversibility |
| Security / risk / compliance | Is the residual risk acceptable? | Data classification, identity, controls, audit, compliance, regulatory exposure |
| Operations / platform / support | Can we run and support this reliably? | Ownership, monitoring, alerts, runbooks, recovery, cost-to-run, support model |

## Facilitation Protocol

The following 60-minute flow can be used for a typical architecture decision meeting.

| Time | Step | Facilitator action | Output |
|---|---|---|---|
| 0-5 minutes | Open the decision | State the decision, why it matters now, and what “done” means for the meeting | Shared decision statement |
| 5-10 minutes | Confirm owner and impact radius | Confirm the decision owner, decision authority, affected scope, and impacted architecture areas | Owner and impact radius |
| 10-25 minutes | Capture stakeholder concerns | Give each stakeholder concern domain focused time before debating the preferred option | Stakeholder concern map |
| 25-35 minutes | Compare options | Compare the preferred option, credible alternatives, and do-nothing or defer options | Options considered |
| 35-43 minutes | Identify evidence gaps | Ask what is still unknown and what evidence is needed before commitment | Evidence gaps |
| 43-50 minutes | Record dissent | Capture objections, unresolved concerns, and the response to each | Dissent log |
| 50-55 minutes | Set decision state | Confirm whether the decision is accepted, conditional, deferred, rejected, escalated, or superseded | Decision state |
| 55-60 minutes | Confirm actions and ADR handoff | Assign follow-up actions, outcome measure, ADR owner, and repository location | Follow-up actions and ADR handoff |

## Facilitation Rules

| Rule | Meaning |
|---|---|
| Concerns before advocacy | Stakeholder concerns are captured before debating the preferred option |
| Evidence before confidence | Strong opinions are tied to evidence or recorded as assumptions |
| Dissent before closure | Disagreement is recorded before the decision state is declared |
| Outcome before documentation | The ADR is not complete until the decision has an outcome measure |

## Decision State

The meeting should end with an explicit decision state.

| Decision state | Meaning | Typical next step |
|---|---|---|
| Proposed | A direction exists, but the decision is not accepted yet. | Complete missing concern review or evidence collection |
| Accepted | The decision is approved without conditions | Write or update the ADR |
| Accepted with conditions | The decision is approved only if named conditions are met | Track conditions as follow-up actions |
| Deferred pending evidence | The decision cannot be made until specific evidence gaps are closed | Assign evidence owners and revisit |
| Rejected | The option is explicitly not being pursued | Record why and identify the remaining path |
| Escalated | The decision exceeds the authority or risk appetite of the meeting | Route to the appropriate governance body or accountable executive |
| Superseded | A later decision replaces this one | Link the old and new ADRs |

Accepted with conditions is not the same as accepted.

## ADR Handoff

The card is used per decision, not per calendar meeting.

A single meeting may produce:

- no ADR if no architecturally significant decision was made
- one ADR if one architecturally significant decision was made
- multiple linked ADRs if several distinct decisions were made
- a proposed or draft ADR if the decision is deferred pending evidence

The unit of an ADR is the decision, not the meeting.

Use the following questions to complete the ADR handoff.

| Question | Output |
|---|---|
| Did this meeting produce an architecturally significant decision? | Yes, no, or deferred |
| How many distinct decisions were made? | Numbered decision list |
| Which decisions need ADRs? | ADR titles or IDs |
| Are any ADRs linked? | Parent, child, related, superseded |
| Who owns each ADR? | Named author or decision owner |
| What is the state of each ADR? | Proposed, accepted, accepted with conditions, deferred, rejected, superseded |

## Finding Better Comparison Areas

Many ADRs compare options across familiar areas such as cost, timeline, security, delivery effort, and support. Those are useful, but they may not expose the most important trade-offs.

A practical technique is to look for the edges of the decision.

Beyond the usual dimensions, the architect should ask:

- What will this decision make harder to change later?
- What other decisions will this trigger?
- Which teams will inherit ownership?
- Which quality attributes will be constrained?
- Which assumptions would cause the most damage if they are wrong?
- What does this option make impossible later?
- Where does this conflict with another decision, standard, or principle?
- Which stakeholder benefits now and which stakeholder pays later?
- What would make this decision reopen?
- What does doing nothing actually cost?

This connects to BTABoK concepts such as decision scope, impact radius, reversibility, information quality, decision cascades, and decision traceability.

## Canvas Sections and Links to BTABoK

The card is divided into sections that follow the natural flow of an architecture decision meeting. The upper sections clarify the decision and its scope. The middle sections make stakeholder concerns and options visible. The lower sections capture evidence, dissent, decision state, follow-up actions, and ADR handoff.

Each section should be completed with enough detail for someone who did not attend the meeting to understand what was decided, why it was decided, what concerns were considered, and what still needs to happen.

![Five-Stakeholder Architecture Decision Meeting Card](/pages/structured_canvases/media/five_stakeholder_architecture_decision_meeting_card.png)

[Download Five-Stakeholder Architecture Decision Meeting Card PPT](/pages/structured_canvases/media/ppt/five_stakeholder_architecture_decision_meeting_card.pptx){:target="_blank"}


| Canvas area | What to put in this area | Related BTABoK concepts |
|---|---|---|
| Decision trigger | Why the decision is needed now. Include deadline, dependency, risk, funding gate, delivery blocker, or governance need. | [Architecturally Significant Decisions](https://iasa-global.github.io/btabok/decisions.html), [Engagement Models](https://iasa-global.github.io/btabok/engagement_models_m.html), governance |
| Decision statement | The decision being made in one clear statement. Include scope, outcome, and known tradeoff. | [Architecture Decision Record](https://iasa-global.github.io/btabok/architecture_decision_record.html), design reasoning, [Requirements](https://iasa-global.github.io/btabok/requirements.html) |
| Decision owner | The person accountable for the decision after the meeting. Include authority route if approval is delegated. | Decision authority, stakeholder management, governance |
| Impact radius | The affected scope: module, product, service, solution, value stream, enterprise, or ecosystem. | Decision scope, impact radius, [Architecture Decision Cascade Card](https://iasa-global.github.io/btabok/architecture_decision_cascade_card.html) |
| ASRs and quality attributes | The architecturally significant requirements, constraints, policies, standards, and quality attributes affected. | [Architecturally Significant Requirements](https://iasa-global.github.io/btabok/asr_card.html), [Quality Attributes](https://iasa-global.github.io/btabok/quality_attributes.html) |
| Stakeholder concern map | Concerns from executive/sponsor, product/customer, engineering/delivery, security/risk/compliance, and operations/platform/support. | Extended team, human dynamics, stakeholder engagement |
| Options considered | Preferred option, credible alternative, do-nothing option, and defer option where relevant. | Tradeoff analysis, [Architecture Decision Record](https://iasa-global.github.io/btabok/architecture_decision_record.html), [Analysis](https://iasa-global.github.io/btabok/analysis.html) |
| Evidence used | Facts that support the decision, such as metrics, estimates, models, prototypes, threat models, cost analysis, or operational data. | Information quality, architecture analysis, decision repository |
| Evidence gaps | Unknowns that affect the decision. Include owner, due date, and decision impact. | Decision quality, risk methods, [Analysis](https://iasa-global.github.io/btabok/analysis.html) |
| Dissent log | Objections or unresolved concerns. Include stakeholder, concern, severity, response, and whether the concern was accepted, mitigated, overruled, or escalated. | Human dynamics, organizational dynamics, governance |
| Decision state | The state of the decision at the end of the meeting. | Decision lifecycle, decision repository, governance |
| Follow-up actions | Actions required after the meeting. Include owner and due date. | Engagement model, architecture practice, governance |
| Outcome measure | How the decision will be reviewed later. Include metric, baseline, target, review date, and trigger to reopen the decision. | Outcomes, value traceability, benefits realization |
| ADR handoff | ADR ID, author, repository location, linked decisions, and review date. | [Architecture Decision Record](https://iasa-global.github.io/btabok/architecture_decision_record.html), decision repository, traceability |

The card should be completed with the minimum detail needed to make the decision reviewable. It should not become a heavy governance artifact. For smaller decisions, some sections may be brief. For larger decisions, especially those with broader impact radius, difficult reversibility, or unresolved stakeholder concerns, the sections should be completed with more rigor.

## Worked Example

### Scenario

A team is deciding whether to use a managed customer identity service for a new external partner portal instead of extending an internal identity platform or building custom authentication.

### Decision Statement

Decide whether to adopt a managed customer identity service for the external partner portal in order to meet launch timing, MFA, auditability, and partner onboarding needs, accepting potential vendor dependency and recurring service cost.

### Stakeholder Concern Map

| Stakeholder concern domain | Concern captured |
|---|---|
| Executive / sponsor / economic buyer | Launch delay has business impact. Recurring cost is acceptable if it avoids two quarters of internal platform work. |
| Product / customer / business owner | Partner onboarding must be simple. Password reset and MFA flows affect adoption and support calls. |
| Engineering / delivery | Managed SDK integration appears feasible, but migration and vendor lock-in need design review. |
| Security / risk / compliance | Data classification, audit logs, MFA policy, and agreement review are mandatory before approval. |
| Operations / platform / support | Service ownership, monitoring, incident routing, and support playbooks must be defined before launch. |

### Options Considered

| Option | Summary |
|---|---|
| Managed customer identity service | Fastest path, stronger built-in controls, but creates recurring cost and vendor dependency |
| Extend internal identity platform | Better internal consistency, but slower delivery and may not support external partner journeys well |
| Build custom authentication | Maximum control, but high risk and poor fit unless identity is a differentiating capability |
| Defer decision | Avoids commitment now, but blocks portal delivery and partner onboarding |

### Evidence Gaps

| Evidence gap | Owner | Due date | Decision impact |
|---|---|---|---|
| Confirm data classification and policy fit | Security lead | Before approval | May change control requirements or approval state |
| Validate SDK integration complexity | Engineering lead | Before sprint planning | May affect delivery estimate |
| Confirm support ownership and incident routing | Operations lead | Before production readiness | May add operational readiness conditions |
| Confirm recurring cost model | Sponsor | Before final ADR | May affect funding approval |

### Dissent Log

| Stakeholder | Concern | Severity | Response |
|---|---|---|---|
| Engineering | Vendor lock-in may make future migration expensive | Medium | Record as accepted tradeoff with migration design note |
| Operations | Support ownership is not yet clear | High | Decision accepted only with operational readiness condition |
| Security | Data classification and audit obligations need validation | High | Decision deferred from accepted state until validation is complete |

### Decision State

Accepted with conditions.

### Conditions

- Security completes data classification and control mapping.
- Engineering completes SDK integration spike.
- Operations defines service ownership, alerting, and incident routing.
- Product confirms onboarding success measure.
- Sponsor accepts recurring cost model.

### Outcome Measure

Partner onboarding completion rate reaches the agreed target within 60 days of launch. Authentication-related support tickets remain below the agreed threshold. No high-severity identity control gaps remain open at production readiness review.

### ADR Handoff

| ADR handoff item | Value |
|---|---|
| ADR title | Adopt managed customer identity service for external partner portal |
| ADR state | Accepted with conditions |
| ADR owner | Solution architect |
| Decision owner | Executive sponsor / economic buyer |
| Linked decisions | Support ownership model, audit logging design, onboarding flow design |
| Review date | 60 days after launch |

## Review Questions

Use these questions to review whether the card was completed with enough rigor.

- Is the decision statement clear enough to approve or reject?
- Is there one named decision owner?
- Is the impact radius understood?
- Are the five stakeholder concern domains represented?
- Were the options compared, not just listed?
- Were do-nothing and defer options considered where relevant?
- Was evidence separated from assumptions?
- Were evidence gaps assigned to owners?
- Was dissent recorded?
- Is the decision state explicit?
- Are follow-up actions clear?
- Is there an outcome measure?
- Is the ADR handoff complete?

## Related BTABoK Concepts

This card is related to the following BTABoK concepts:

- [Architecturally Significant Decisions](https://iasa-global.github.io/btabok/decisions.html)
- [Architecture Decision Record](https://iasa-global.github.io/btabok/architecture_decision_record.html)
- [Architecturally Significant Requirements](https://iasa-global.github.io/btabok/asr_card.html)
- [Requirements](https://iasa-global.github.io/btabok/requirements.html)
- [Quality Attributes](https://iasa-global.github.io/btabok/quality_attributes.html)
- [Analysis](https://iasa-global.github.io/btabok/analysis.html)
- [Architecture Decision Cascade Card](https://iasa-global.github.io/btabok/architecture_decision_cascade_card.html)
- [Structured Canvases](https://iasa-global.github.io/btabok/structured_canvases_m.html)
- [Engagement Models](https://iasa-global.github.io/btabok/engagement_models_m.html)
```

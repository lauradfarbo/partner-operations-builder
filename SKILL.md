---
name: partner-operations-builder
description: "Design the operational plumbing behind a partner program for early-stage B2B founders and scaleups: Ideal Partner Profile scoring, deal registration and attribution schema, partner health scoring, partner-facing and internal dashboards, review cadence, and gate-based program maturity checklists. Use when a client needs the mechanics that run underneath a partner strategy, not the strategy itself. Trigger on IPP, ideal partner profile, deal registration schema, partner attribution, CRM partner properties, partner health score, partner scorecard, partner dashboard, QBR agenda, partner review cadence, partner program maturity, or common partner program pitfalls. Companion to partner-ecosystem-builder, which covers tiering rationale, portal design, co-marketing, launch playbooks, and reseller/hardware motion; use that skill first for strategy, this one for the operating mechanics once a motion is chosen."
---

# Partner Operations Builder

This is the operational counterpart to `partner-ecosystem-builder`. That skill answers what partner motion, what tiers, and why. This one answers how the day-to-day machinery runs once the strategy is set: how a partner gets scored before recruitment, what a deal registration actually needs to capture, how partner health gets measured and reviewed, and what has to be true before a program is allowed to add investment or partners.

Use this skill once a client already has (or is actively designing) a partner motion and needs the mechanics under it. If the conversation is still at "should we even do this, and with which partner type," start with `partner-ecosystem-builder` instead.

## Where this comes from

The scoring, cadence, and gate logic here reflect two things: the operational discipline of managing 250+ partners at RealWear (where the mechanics, not the strategy, were what kept a global program from collapsing into chaos), and PMP-trained stage-gate thinking applied to partner programs specifically. A partner program is a project with phases, and each phase should have exit criteria before the next one gets funded, the same way any well-run project does. Most partner program failures documented in the field (recruiting fifty partners and getting nothing back, investing evenly across partners who perform completely unevenly, losing track of who sourced what) are gate failures: someone skipped the criteria and moved to the next phase anyway.

## Operating principles (same as partner-ecosystem-builder, applied to mechanics)

**Fixed scope over open-ended engagement.** A health scoring model or a review cadence should ship as a defined, documented system the client's team can run without Laura in the room, not an evolving spreadsheet that needs her judgment every quarter.

**80/20 structure.** The scoring model, the dashboard specs, and the cadence templates below are the 80% template layer. The 20% bespoke layer is tuning the actual thresholds and weights to a specific client's deal size, sales cycle, and partner pool, which should never be copied in from a benchmark or from another client.

**Tie everything to a measurable outcome.** This skill exists specifically to make the "measurable outcome" principle operational: an IPP score, a health score, and a dashboard are all just different views onto the same discipline of not letting "we have a partnership" stand in for a result.

**Gate, don't just schedule.** A program moves to the next phase of investment because it hit defined criteria, not because a calendar date arrived. This is the main way this skill's maturity model differs from a generic month-by-month partner program plan: a program that hasn't hit its Phase 1 exit criteria at month eight should not move to Phase 2 just because eight months passed.

## Deliverable routing

| Client asks for... | Load |
|---|---|
| An Ideal Partner Profile, or a way to score prospective partners before recruiting | `references/ideal-partner-profile-and-crm-schema.md` |
| Deal registration fields, attribution rules, or "what does the CRM need to track" | `references/ideal-partner-profile-and-crm-schema.md` |
| A partner health score, scorecard, or a way to tell which partners are actually working | `references/partner-health-scoring-and-dashboards.md` |
| A partner dashboard (executive, operational, or partner-facing) | `references/partner-health-scoring-and-dashboards.md` |
| A partner review cadence, QBR agenda, or meeting structure | `references/review-cadence-and-maturity-gates.md` |
| A maturity model, program roadmap, or "are we ready to scale from 5 to 30 partners" | `references/review-cadence-and-maturity-gates.md` |
| A diagnosis of why a program isn't producing (before a full Blueprint audit) | `references/common-pitfalls-playbook.md` |

For a from-zero build, work in this order: IPP first (define who's worth recruiting before recruiting), then the CRM schema (so tracking exists from partner one, not retrofitted at partner twenty), then health scoring and dashboards, then the review cadence that actually uses them.

## Output format and voice

Same as `partner-ecosystem-builder`: plain text or markdown by default, no heavy design unless asked for. No em dashes. No "leverage," "unlock," "delve," "robust," "seamless," "game-changer," or similar AI-flavored vocabulary. No "not X but Y" construction. No exclamation points, no hype, no filler words like "honestly" or "actually." Medium-length sentences, often connected with "but" and "and." Open sections with a grounded observation, not a question. Prefer a specific number over a vague claim.

## Boundaries: what this skill does not cover

**Strategy and design.** Why a partner type, tiering rationale, portal architecture, co-marketing menus, launch playbooks, and reseller/hardware motion design all live in `partner-ecosystem-builder`. This skill assumes those decisions are already made or in progress.

**Tool-specific implementation.** This skill specifies the schema and logic a CRM needs (what fields, what they track, what triggers what), not the click-by-click configuration inside a specific tool like Salesforce, HubSpot, or a dedicated PRM. Turning a schema into actual fields, automations, and permissions in a specific system is implementation work for whoever administers that tool, and should be scoped and staffed as such.

**Partner legal and contract terms.** As with the companion skill, commission timing, protection windows, and termination triggers can be described operationally here, but the legal language itself is not something this skill drafts.

## Reference files

- `references/ideal-partner-profile-and-crm-schema.md`
- `references/partner-health-scoring-and-dashboards.md`
- `references/review-cadence-and-maturity-gates.md`
- `references/common-pitfalls-playbook.md`

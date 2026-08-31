# Partner Operations Builder

A Claude skill for the operational plumbing behind a partner program, built by [Laura Farbo](https://www.linkedin.com/in/laurafarbo). Companion to `partner-ecosystem-builder`.

## What this is

`partner-ecosystem-builder` answers what partner motion to run and why. This skill answers how the mechanics underneath it actually work day to day: how a prospective partner gets scored before recruitment, what a deal registration needs to capture to make attribution possible, how partner health gets measured, what a partner review cadence should look like, and what has to be true before a program earns the right to add investment or partners.

The gate-based maturity model here reflects PMP-trained stage-gate thinking applied to partner programs specifically: a program advances because it met defined exit criteria, not because a certain number of months passed. The health scoring, cadence, and schema come out of running operational discipline across a 250+ partner global program at RealWear, where mechanics, not strategy, were what kept the program from collapsing into chaos at scale.

## How it's structured

- `SKILL.md`: scope, boundary against the strategy-focused companion skill, and a routing table to the right reference file for a given deliverable.
- `references/ideal-partner-profile-and-crm-schema.md`: the IPP scoring template for screening prospective partners, plus the deal registration and attribution schema a CRM (or a spreadsheet, early on) needs to carry.
- `references/partner-health-scoring-and-dashboards.md`: a weighted partner health scoring model, and three separate dashboard specs (executive, operational, partner-facing).
- `references/review-cadence-and-maturity-gates.md`: a weekly-through-annual review cadence, and a gate-based (not calendar-based) program maturity model with explicit exit criteria per phase.
- `references/common-pitfalls-playbook.md`: a fast diagnostic reference for the failure patterns that show up most often in a stalled program, useful before deciding whether a full audit is warranted.

## Relationship to partner-ecosystem-builder

Use `partner-ecosystem-builder` first for strategy: which partner type, why now, how tiers and portal content should work, co-marketing and launch design, reseller/hardware motion. Use this skill once that motion is chosen and needs the operating mechanics underneath it. Neither skill duplicates the other by design; each stays self-contained rather than depending on files installed as part of the other.

## What this skill doesn't cover

Partner strategy and design (see the companion skill), tool-specific CRM configuration (this skill specifies the schema and logic, not the click-by-click setup inside Salesforce, HubSpot, or a PRM), and partner legal or contract drafting.

## Using it

Install as a Claude skill. It triggers on requests involving an Ideal Partner Profile, deal registration schema, CRM partner properties, partner health scoring, partner dashboards, QBR agendas, review cadence, program maturity, or diagnosing why a partner program isn't producing.

## License

MIT. See `LICENSE`.

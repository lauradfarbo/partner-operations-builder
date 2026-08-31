# Ideal Partner Profile and CRM Schema

## Ideal Partner Profile (IPP)

An IPP exists to answer one question before any recruiting starts: what does a good partner actually look like for this specific client, so time doesn't get spent signing partners who were never going to produce.

### Scoring structure

Score a prospective partner across three groups of criteria, each on a 1-5 scale. Keep the groups; adjust the specific criteria inside them to the client's actual motion (a reseller's operational readiness looks different from a technology partner's).

**Strategic fit.** Does this partner's audience overlap with the client's actual buyer, is the offering complementary rather than competitive, does the partner's go-to-market motion match the client's (a partner running high-touch enterprise sales doesn't pair well with a client selling self-serve, and vice versa), and is there geographic or vertical alignment if that matters for this client.

**Operational readiness.** Does the partner have a dedicated team or person who'd actually own this relationship, is there a CRM or tracking system on their side capable of registering deals, do they have an existing customer base worth cross-selling into, and do they have real marketing capability (content, events, an audience) rather than just a logo.

**Commitment signals.** Is there an identified executive sponsor on the partner's side, will they invest time or budget in enablement, have they referred deals informally before (the single strongest predictor of future referrals), and is there a strategic reason for them to want this beyond the commission check.

### Setting the threshold

Score each candidate partner 1-5 on each criterion within the three groups (adjust the exact criteria count per group to the client's situation, but keep the three groups). Total the score. Where the tier lines fall depends entirely on the client's actual partner pool and deal economics, not on an imported number: pull whatever data exists on partners already in motion, rank them, and set the top-tier threshold just above current best performance. A client with no partners yet should treat the first cohort's scores as a hypothesis to recalibrate after 90 days, not a fixed rule.

Refuse to recruit anyone who can't be scored, meaning a partner conversation that's all enthusiasm and no evidence on operational readiness or commitment signals isn't ready to be recruited yet. It's ready for one more conversation to surface that evidence.

## Deal registration and attribution schema

This is the schema a CRM (or a spreadsheet, at the earliest stage) needs to carry so that partner-sourced and partner-influenced pipeline can be reported with any confidence. Build this before recruiting partner three, not after discovering at partner twenty that nothing has been tracked.

### Core fields

- **Partner sourced** (yes/no): the partner originated the opportunity, meaning the first real conversation happened because of their introduction.
- **Partner influenced** (yes/no): the client's own team originated the deal, but the partner actively helped move it.
- **Partner name** (linked record): which partner, not a free-text field that drifts into five spellings of the same company.
- **Partner contact**: who at the partner is actually involved, since "the partner" isn't a person.
- **Registration ID** (auto-generated): a unique reference for the registration itself, separate from the deal ID, so a registration's history survives even if the deal record changes.
- **Registration date** and **registration expiry** (auto-calculated from a defined protection window): when the clock started and when protection lapses if nothing progresses.
- **Commission rate** and **commission amount** (rate pulled from tier, amount calculated from deal value times rate): so payout isn't a manual lookup every time.
- **Partner tier**: which tier the partner sits in at the time of registration, since tier can change and the rate that applied at registration should be traceable.

### Registration process

1. Partner submits a registration (through a portal form, a simple web form, or at minimum a defined email format) with account name, contact, estimated value, and timeline.
2. An automatic check against existing pipeline: is this account already an active opportunity. If yes, the conflict resolution rule below applies. If no, register and assign.
3. A partner-side owner (partner manager, or the founder in an early-stage program) reviews within a defined window, commonly 24 to 48 hours. Slow review is one of the fastest ways to erode partner trust in the process.
4. The registration holds for a defined protection window (60 to 120 days depending on deal size and sales cycle; a longer cycle needs a longer window). If the deal hasn't progressed by expiry, the registration lapses and can be re-registered if the partner is still engaged.

### Conflict resolution rule

Decide this before the first conflict, not during it. A workable default: first to register wins, within a short grace period (commonly 5 to 7 days) that accounts for a partner and a direct rep independently reaching the same account around the same time. If an account already has an open opportunity when a partner registers it, direct sales owns the deal unless the partner can show evidence of a prior relationship. If both sides are genuinely engaged, the deal becomes a co-sell with an agreed split rather than a fight over full ownership. Set an escalation path (partner manager plus sales manager, resolving within 48 hours) and use it, rather than letting conflicts sit unresolved while both sides quietly keep working the account.

## A note on implementation

This is a schema and a set of rules, not a build guide for a specific CRM. Turning "partner sourced" into an actual checkbox field with the right automation behind it in Salesforce, HubSpot, or a PRM tool is implementation work, and the right person for that job is whoever administers the client's actual system. What this reference guarantees is that the fields and logic they build will actually answer the attribution question, instead of producing a CRM that looks thorough but still can't tell anyone where a deal came from.

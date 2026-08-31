# Partner Health Scoring and Dashboards

## Why score partner health at all

A tier tells you what a partner earned in the past. A health score tells you what's happening right now, and it's the earlier warning signal. A partner can hold Builder tier status from last quarter's performance while quietly going inactive this quarter, and a health score catches that before the next tier review does.

## The health scoring model

Score each partner 0-100 across four weighted dimensions. The weights below are a starting point, not a fixed rule; adjust them to reflect what actually predicts a healthy partner for this specific client's motion (a technology partner's health looks different from a reseller's, and the dashboard reference below assumes the underlying data supports whichever weighting is chosen).

**Pipeline activity (35%).** Deal registrations this quarter, pipeline value created, and deals actually progressing through stages rather than sitting stalled. This is weighted highest because activity is the leading indicator; revenue lags it by a quarter or two.

**Revenue production (25%).** Closed-won revenue over the trailing twelve months, win rate on registered deals, and average deal size. This is the lagging confirmation that the activity is converting.

**Engagement (20%).** Portal logins and content usage, training or certification completion, event attendance, and responsiveness to outreach. Low engagement combined with high pipeline activity usually means the relationship is transactional rather than durable, worth watching even if current numbers look fine.

**Relationship depth (15%).** Executive sponsor still engaged, QBR attendance, joint planning actually completed rather than scheduled and skipped, and escalation frequency (fewer escalations is healthier, not more).

**Strategic fit (5%).** How well the partner's ICP and market motion still overlap with the client's, since fit can drift as either company's product or market changes even if the relationship itself stays warm.

### Reading the score

- 80 and above: healthy. This is where continued or increased investment makes sense.
- 50 to 79: watch. Something specific is soft, usually engagement or relationship depth even when revenue still looks acceptable. Diagnose which dimension is dragging the score down before deciding what to fix.
- Below 50: at risk. This needs a direct conversation about what's not working, and a real decision about whether to invest in a turnaround or wind the relationship down, rather than letting it drift.

### Review frequency by tier

Score top-tier partners quarterly, mid-tier partners twice a year, and entry-tier partners annually, unless something (a sudden drop in activity, a lost champion, a competitor deal) triggers an off-cycle look. Scoring every partner every month is usually more process than the program can sustain, and it doesn't catch problems any faster than the quarterly cycle does.

## Three dashboards, three audiences

Building one dashboard and showing it to everyone usually means it's wrong for at least two of the three audiences. Build these as three separate views, even if they pull from the same underlying data.

### Executive dashboard

What leadership needs to see without digging: partner-sourced pipeline and revenue (in currency and as a percentage of total), partner-influenced pipeline and revenue, what percentage of all partners are actually producing pipeline (not just signed), the top five partners by contribution, deal registration volume and its conversion rate, and program ROI (attributed revenue divided by program cost). This is the view that answers "is this worth what we're spending on it," and it should answer that question in under a minute of looking at it.

### Operational dashboard

What the partner manager needs to run the program day to day: registrations this month broken out by partner and tier, the registration-to-closed-won conversion rate, average deal size and sales cycle for partner deals versus direct, win rate for partner-sourced versus direct, and partner activity signals (portal logins, content downloads, certification completions) that predict health scores before the quarterly scoring catches up to them.

### Partner-facing dashboard (inside the portal)

What a partner should be able to see about their own standing, without needing to ask: their registered deals and current status, commission earned (paid and pending, since ambiguity here is one of the fastest ways to lose trust), their certification status, their tier and what it would take to move up, and any shared account mapping results relevant to them. A partner with no visibility into their own status will eventually stop trusting the registration process, regardless of how well it actually works on the client's side.

## Tying this back to the one-number principle

A health score and three dashboards can start to feel like the point of the exercise. They aren't. The point is still the single number each partner motion is judged against (see the 1-1-1-1 filter in `partner-ecosystem-builder`). The dashboards exist to make that number visible and current, not to become a reporting project in their own right. If building the dashboard is taking longer than the partner program itself has been running, that's a sign to simplify, not to add more views.

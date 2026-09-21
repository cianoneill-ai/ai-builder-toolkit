---
name: automation-map-intake
description: Run a structured discovery interview with a small business and turn the answers into a ranked automation blueprint with effort, payoff and build order
category: Business & operations
---

# Automation Map intake

Use this when a business owner or operator asks "what should we automate", or when preparing the Automation Map (two sessions, one ranked blueprint). It runs the interview, scores the candidates and writes the blueprint.

## 1. The interview (session one, 60 to 90 minutes)

Ask in this order. Write down verbatim answers, not summaries.

**The week**
- Walk me through last Monday, hour by hour. Who did what.
- Which job came up more than once? Which one did you dread?
- What did someone do by hand that a machine already has the data for?

**The handoffs**
- Where does information move between people or tools (email to spreadsheet, chat to CRM, invoice to accounting)?
- Where does it get re-typed?
- Where does it wait? For how long?

**The failures**
- What went wrong in the last month because someone forgot, or was late, or copied the wrong thing?
- What would break first if the busiest person took two weeks off?

**The tools**
- List every tool you pay for. Which ones does nobody open?
- What is in Google Sheets that should not be?

**The constraints**
- What must never be automated (money out, client-facing promises, anything legal)?
- Who has to approve a change before it goes live?

## 2. Build the candidate list

Every recurring job, handoff or failure from the interview becomes a candidate. Aim for 15 to 30. For each, record: trigger, input, output, who does it now, how often, minutes per occurrence.

## 3. Score (return on effort)

Score each 1 to 5:
- **Hours saved per month** (frequency × minutes, converted).
- **Error cost**: what a mistake in this job costs when it happens.
- **Data readiness**: is the input already digital and structured.
- **Tool fit**: can it be done with free tools or tools already paid for.
- **Risk**: 5 is safe to automate fully, 1 needs a human on every run.

Return on effort = (hours + error cost + reach) ÷ (5 − data readiness + 5 − tool fit + 1). Rank by it. Mark anything with risk ≤ 2 as "human in the loop, always".

## 4. Build order

Not the highest score first. Order by:
1. Something visible within a week (a daily summary, a triage, a report) so the team trusts the process.
2. The highest return-on-effort items that share a data source, built together.
3. Anything that needs a new tool or an approval, last.

## 5. The blueprint (session two deliverable)

```
# Automation Map: <company>

## The three jobs eating the most time
1. <job>: <hours/month>, done by <who>. Automate: yes / partly / no.
...

## Ranked list
| # | Job | Trigger | Hours/mo | Risk | Tools | Build order |

## Do not automate
- <job>: <why>

## Build plan
Week 1: ...
Weeks 2–4: ...
Later: ...

## What you will own
Tools, credentials, the runbook, the person who presses stop.
```

## 6. Rules

- The client keeps the blueprint whether or not any build follows.
- Free or already-paid tools before new subscriptions. Check trial terms before recommending anything.
- Every automation gets an outcome test written into the plan: how we prove it did the thing.
- Nothing that sends, pays, posts or deletes runs without a human review step in version one.

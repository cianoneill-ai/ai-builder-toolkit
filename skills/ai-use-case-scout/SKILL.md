---
name: ai-use-case-scout
description: Find, vet and rank real AI use cases from the open web twice a week, and hand back three worth building or writing about, with sources
category: Research & content
---

# AI use case scout

Use this when the user says "find me AI use cases", "what should I build next", "scout this week", or on a schedule. The job is to come back with three use cases that a non-engineer could build in a weekend, each with evidence that someone has actually done it.

## 1. Where to look (in this order)

- Builder communities: Hacker News "Show HN", r/LocalLLaMA, r/selfhosted, r/ClaudeAI, r/ChatGPTPro, Indie Hackers.
- Release notes and changelogs of the tools the user already runs (agent frameworks, model providers, connectors). New capability = new use case.
- Job boards and "we're hiring" pages in the user's industry. A role that is 80% repeatable work is a use case.
- Support forums for the user's own tools (Shopify, Google Workspace, Telegram bots). Complaints are use cases.
- Newsletters and podcasts in the niche, but only for leads, never as the only source.

Search at least five sources. Log every candidate with a URL before scoring anything.

## 2. Disqualify first

Cut a candidate before scoring if any of these is true:
- Needs code the user cannot read or maintain (a full app, a custom model, anything with a build pipeline).
- Depends on a paid tool with no free tier, or a tool that charges after a trial.
- Cannot be tested for outcome (no way to prove it did the thing, not just responded).
- Is a demo, not a system. If nobody is running it daily, it is a demo.
- Touches money, medical, legal or identity data without a human in the loop.

## 3. Score what survives (0 to 3 each)

- **Pain**: how often the job recurs and how much it costs in hours.
- **Proof**: someone has run it for a month or more, with a write-up or repo.
- **Reach**: how many people in the user's audience have the same problem.
- **Buildability**: free tools, existing connectors, a weekend of describing and testing.
- **Story**: is there a failure or a surprise in it worth writing about.

Rank by total. Ties go to the one with the better story.

## 4. Output

Return exactly this, nothing else:

```
## Scout: <date>

### 1. <use case name>  (score 13/15)
What it does: one sentence.
Who has it: <name/link>, running since <when>.
Build: tools, connectors, the outcome test you'd write.
Cost to run: free / cents a day / say what it is.
Story angle: the one thing that will break or surprise.
Source: <url>

### 2. ...
### 3. ...

### Cut and why
- <candidate>: <disqualifier>
```

## 5. Rules

- Every claim has a URL. No URL, no claim.
- Never invent metrics. If the source gives a number, quote it. If not, say "no numbers published".
- Prefer boring and running over clever and new.
- If fewer than three survive, say so. Do not pad.

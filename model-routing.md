# Model routing by job type

Three tiers, one rule each. Use your provider's current small, mid and frontier models; the names change every few months, the logic doesn't.

| Job | Tier | Why |
|---|---|---|
| Classify or route a request | Small | High volume, easy to check |
| Extract fields, reformat, tag | Small | Deterministic, low stakes |
| Short summaries, yes/no checks | Small | Cheap to verify |
| First drafts (emails, posts, docs) | Mid | Quality matters, you'll edit anyway |
| Research synthesis | Mid | Needs judgement, not genius |
| Routine code changes | Mid | Tests will catch mistakes |
| Architecture and system design | Frontier | Wrong answers are expensive |
| Debugging something subtle | Frontier | Needs deep reasoning |
| Strategy and big decisions | Frontier | Low volume, high stakes |
| Final review before anything ships | Frontier | Last line of defence |

## Rules

- **Route first.** A small model classifies each request and hands it to the right tier.
- **Escalate on failure, not by habit.** Mid tier first; frontier only when a check fails or the stakes are high.
- **Review fallback chains.** Know what takes over when a model is down.
- **Date your config.** Review model versions and prices monthly. Routing on stale prices is guessing.

Background: [Stop paying frontier prices for formatting](https://cianoneill.ai/writing/model-routing-by-job-type/).

# The self-hosted agent security checklist

Run this against any personal agent setup: OpenClaw, a home-built stack, anything with scheduled jobs and tool access. Budget an hour. Each check is a yes or no.

## Secrets

1. **No credentials in config files.** API keys and bot tokens live in a secrets store or environment variables, never in a file agents can read.
2. **Exposed keys are rotated.** If a key ever sat in plain text, assume it leaked. Rotate it.
3. **One key per job where the provider allows it.** When something goes wrong you can revoke one thing, not everything.

## Containment

4. **The sandbox is on, and failures are loud.** If the sandbox can switch itself off on an error, make sure you get an alert when it does.
5. **Commands are allowlisted.** Agents can only execute commands on an explicit list. Everything else is denied.
6. **Tools are scoped per agent.** The content agent does not need shell access. The research agent does not need to send email.

## Inputs

7. **Every chat channel requires a mention or an allowlist.** No open DMs or group policies on bots that can take actions.
8. **Web content is treated as untrusted.** Anything an agent reads from the web can contain instructions. It must never be able to trigger an outbound action directly.

## Outputs

9. **A human approves anything that leaves the building.** Emails, posts, payments, deletions. Research can be autonomous; outbound cannot.
10. **Outbound recipients are allowlisted.** Scheduled jobs can only send to addresses you have approved in advance.

## Models and memory

11. **Fallback chains are reviewed.** You know exactly which model takes over when your first choice is down, and you chose it on purpose.
12. **Memory is pruned on a schedule.** What agents remember and can write back is reviewed monthly, and anything sensitive is removed.

---

Scored under 9? Fix secrets and outbound first. That is where the real damage comes from. The full story of my own audit: [I audited my own AI agent](https://cianoneill.ai/writing/i-audited-my-own-agent/).

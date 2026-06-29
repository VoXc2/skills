# Dealix Skills Pack

## Executive verdict

The `skills` repository is best treated as a **distribution layer for agent operating procedures**, not as the main Dealix product repository.

Dealix should use this repo to package repeatable operating knowledge into installable `SKILL.md` modules that can be consumed by Claude Code, Codex, Cursor, OpenCode, Kimi Code, Roo, Continue, and other supported agents.

## Why this matters for Dealix

Dealix is not just a chatbot, CRM, or dashboard. Dealix is a Saudi B2B AI Operating Systems company. Its work must become repeatable across agents and environments.

This pack turns Dealix's operating doctrine into portable skills:

1. Revenue Command Room OS
2. Company Brain OS
3. Client Growth Operator OS
4. Client Delivery OS
5. Loop Operating System
6. Trust and Outbound Safety OS
7. Release Engineer OS

## How these skills should be used

Install them into a target repo, then assign the right skill to the right agent task.

Example:

```bash
npx skills add VoXc2/skills --skill dealix-revenue-command-room
npx skills add VoXc2/skills --skill dealix-company-brain-os
npx skills add VoXc2/skills --skill dealix-release-engineer
```

Use a skill without installing:

```bash
npx skills use VoXc2/skills --skill dealix-client-growth-operator | claude
```

## Operating rules

These rules are mandatory across all Dealix skills:

- Do not enable live outbound by default.
- Keep external sending behind approval gates.
- Do not create fake ROI, fake clients, fake testimonials, or guaranteed revenue claims.
- Require source URLs and verification status for outreach targets.
- Require human review for WhatsApp, email, LinkedIn, calls, contracts, discounts, and pricing commitments.
- Prefer small PRs over giant unreviewable dumps.
- Produce proof packs and reports after every operating loop.
- Treat generated reports/outbox artifacts as runtime outputs unless intentionally committed.

## Recommended skill stack for Dealix repo work

| Work type | Skill |
|---|---|
| Stabilizing CI, build, release branches | `dealix-release-engineer` |
| Running daily sales machine | `dealix-revenue-command-room` |
| Turning signals into daily decisions | `dealix-company-brain-os` |
| Preparing client outreach actions | `dealix-client-growth-operator` |
| Delivering a client sprint | `dealix-client-delivery-os` |
| Building durable agent loops | `dealix-loop-operating-system` |
| Reviewing claims, privacy, and outbound | `dealix-trust-and-outbound-safety` |

## Implementation quality bar

A Dealix skill is acceptable only if it gives the agent:

- when to use it
- what files to inspect
- what to create or update
- safety constraints
- validation commands
- definition of done
- final report requirements

## Future expansion

Next useful skills:

- `dealix-hubspot-os`
- `dealix-railway-production-ops`
- `dealix-saas-foundation`
- `dealix-website-brand-os`
- `dealix-market-watch-os`
- `dealix-proof-pack-os`

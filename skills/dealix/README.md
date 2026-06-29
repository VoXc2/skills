# Dealix Agent Skills

This directory contains the Dealix operating skill pack for agent-based work.

## Skills

| Skill | Purpose |
|---|---|
| `dealix-release-engineer` | Stabilize branches, PRs, CI, build, Railway, and safe release gates |
| `dealix-revenue-command-room` | Run target scoring, drafts, follow-ups, proposal briefs, and revenue reports |
| `dealix-company-brain-os` | Convert operating signals into daily founder decisions and weekly memos |
| `dealix-client-growth-operator` | Prepare controlled channel actions for email, WhatsApp, LinkedIn, phone, and proposals |
| `dealix-client-delivery-os` | Deliver client work through intake, diagnosis, scope, blueprint, proof pack, and handoff |
| `dealix-loop-operating-system` | Convert scattered scripts into bounded operating loops with verifiers and reports |
| `dealix-trust-and-outbound-safety` | Review claims, privacy, consent, opt-out, approval cards, and outbound policy gates |

## Install examples

```bash
npx skills add VoXc2/skills --skill dealix-release-engineer
npx skills add VoXc2/skills --skill dealix-revenue-command-room
npx skills add VoXc2/skills --skill dealix-company-brain-os
```

Install all Dealix skills:

```bash
npx skills add VoXc2/skills --skill '*' --full-depth
```

Use one skill without installing:

```bash
npx skills use VoXc2/skills --skill dealix-client-growth-operator | claude
```

## Dealix safety baseline

Every Dealix skill assumes these defaults unless a separate controlled-live implementation is explicitly approved:

```env
EXTERNAL_SEND_ENABLED=false
EMAIL_SEND_ENABLED=false
WHATSAPP_SEND_ENABLED=false
WHATSAPP_ALLOW_LIVE_SEND=false
SMS_SEND_ENABLED=false
OUTBOUND_MODE=draft_only
```

## Recommended use

Use the skills in this order for Dealix repo execution:

1. `dealix-release-engineer`
2. `dealix-loop-operating-system`
3. `dealix-revenue-command-room`
4. `dealix-company-brain-os`
5. `dealix-client-growth-operator`
6. `dealix-client-delivery-os`
7. `dealix-trust-and-outbound-safety`

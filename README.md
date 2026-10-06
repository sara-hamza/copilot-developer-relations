# copilot-developer-relations

## What it does

Developer Assistant: requirements summaries, open items, stakeholder questions and handover prep for property developments.

Part of the **department-copilots** suite: local-only copilots where the employee provides the input, Claude analyses it on the machine, and the employee decides what to do. No CRM, NMS, email or system integrations.

## Install

```bash
claude plugin marketplace add sara-hamza/department-copilots
```

```bash
claude plugin install developer-relations@department-copilots
```

Paste the development plan details, your project notes, the developer's latest requests or the design constraints, and get back a requirements summary, a tracked open-items list, a clean question list for the developer, or the internal handover pack to delivery.

| Command | Use when |
|---|---|
| `/developer-relations:requirements <paste or file>` | Summarise what the development needs: premises, staging, dates, constraints, open items, questions, risks |
| `/developer-relations:open-items <paste>` | Tracked list of open items with owner and due; flags stale and ownerless |
| `/developer-relations:developer-questions <paste>` | Clear, grouped question list to send the developer (civil, staging, pit and pipe, comms room, power, easements, titles and dates) |
| `/developer-relations:handover <paste or files>` | Internal handover pack from BD or developer relations to the delivery team, with present and missing marked |

Requires `copilot-common` (privacy rules, document-reader for development plans and civil drawings exported as PDF, spreadsheet-reader for lot schedules and stage programmes, writing-helper for the developer tone).

Reference knowledge lives in `skills/developer-assistant/references/`. Civil specification names, lead times, siting requirements and internal contacts are sensible defaults marked `CUSTOMISE`.

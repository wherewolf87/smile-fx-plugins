# SMILE-FX® Customer Support

> Triages questions, drafts replies, packages escalations and turns resolved questions into help articles.

**Install id:** `sfx-customer-support` | **Version:** 1.0.0 | **Skills:** 5 | **Commands:** 0 | **Licence:** Apache-2.0

## Who it is for

Front desk and patient experience teams who answer questions by email, chat or help desk.

## Install

**Claude Code.** In a session:

```text
/plugin marketplace add wherewolf87/smile-fx-plugins
/plugin install sfx-customer-support@smile-fx-plugins
```

The install command opens the plugin panel so you can review it and pick a scope. From your shell, use `claude plugin marketplace add wherewolf87/smile-fx-plugins` and `claude plugin install sfx-customer-support@smile-fx-plugins`.

**Cowork.** Open **Customize**, then **Plugins**, then **Add marketplace**, and enter `wherewolf87/smile-fx-plugins`. Select **SMILE-FX Customer Support** and **Install**, then connect your tools on its **Connectors** tab. Plugins need a paid Claude plan.

Full steps: [install guide](../README.md#install).

## Try asking

- "Sort these five inbound questions by urgency."
- "Draft a warm, plain reply to this billing question."
- "Turn this resolved question into a help article."

## Skills (5)

Claude uses a skill when your request matches it. You can also call one by name.

| Skill | What it does |
|---|---|
| `/sfx-customer-support:customer-escalation` | Packages an escalation with full context for the right team. |
| `/sfx-customer-support:customer-research` | Researches a customer question across sources, with attribution. |
| `/sfx-customer-support:draft-response` | Drafts a customer reply suited to the situation and relationship. |
| `/sfx-customer-support:kb-article` | Turns a resolved issue or common question into a help article. |
| `/sfx-customer-support:ticket-triage` | Sorts and prioritizes a ticket or customer issue. |

## Connectors

Set up: Slack, Intercom, HubSpot, Guru, Atlassian (Jira, Confluence), Notion. Blank on purpose, connect them yourself: Google Calendar, Gmail.

Each connector signs in with your own account, and nothing connects until you do. [CONNECTORS.md](CONNECTORS.md) lists what each one needs.

## Good to know

- Remove patient details from a message before you paste it, unless your plan is covered by a signed BAA.
- Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.
- Software suggests. People decide. Check what a skill produces before you use it.

## Credits and licence

Adapted by SMILE-FX P.A. from the `customer-support` plugin in Anthropic's [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) (commit `da38ec1`), under the Apache License 2.0. SMILE-FX changed the plugin name and metadata, this README, the connector notes, and skill text that named the old plugin. The changes are listed in [MODIFICATIONS.md](../MODIFICATIONS.md). Licence: [LICENSE](LICENSE). Notices: [NOTICE](../NOTICE).

© 2026 SMILE-FX P.A. SMILE-FX® is a registered trademark of SMILE-FX P.A. SMILE-FX P.A. is not affiliated with, sponsored by or endorsed by Anthropic. Anthropic, Claude, Claude Code and Cowork are trademarks of Anthropic and are named here only to describe compatibility.

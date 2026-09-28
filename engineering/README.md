# SMILE-FX® Engineering

> Supports standups, code review, debugging, architecture decisions, incident response and technical documentation.

**Install id:** `sfx-engineering` | **Version:** 1.0.0 | **Skills:** 10 | **Commands:** 0 | **Licence:** Apache-2.0

## Who it is for

Practices or groups with in-house developers or an IT partner.

## Install

**Claude Code.** In a session:

```text
/plugin marketplace add wherewolf87/smile-fx-plugins
/plugin install sfx-engineering@smile-fx-plugins
```

The install command opens the plugin panel so you can review it and pick a scope. From your shell, use `claude plugin marketplace add wherewolf87/smile-fx-plugins` and `claude plugin install sfx-engineering@smile-fx-plugins`.

**Cowork.** Open **Customize**, then **Plugins**, then **Add marketplace**, and enter `wherewolf87/smile-fx-plugins`. Select **SMILE-FX Engineering** and **Install**, then connect your tools on its **Connectors** tab. Plugins need a paid Claude plan.

Full steps: [install guide](../README.md#install).

## Try asking

- "Review this pull request."
- "Write a postmortem for yesterday's website outage."
- "Create a deploy checklist for our booking site."

## Skills (10)

Claude uses a skill when your request matches it. You can also call one by name.

| Skill | What it does |
|---|---|
| `/sfx-engineering:architecture` | Creates or evaluates an architecture decision record. |
| `/sfx-engineering:code-review` | Reviews code changes for security, performance and correctness. |
| `/sfx-engineering:debug` | Runs a structured debugging session: reproduce, isolate, diagnose and fix. |
| `/sfx-engineering:deploy-checklist` | Runs a pre-deployment verification checklist. |
| `/sfx-engineering:documentation` | Writes and maintains technical documentation. |
| `/sfx-engineering:incident-response` | Runs an incident: triage, communication and postmortem. |
| `/sfx-engineering:standup` | Writes a standup update from recent activity. |
| `/sfx-engineering:system-design` | Designs systems, services and architectures. |
| `/sfx-engineering:tech-debt` | Finds, sorts and prioritizes technical debt. |
| `/sfx-engineering:testing-strategy` | Designs test strategies and test plans. |

## Connectors

Set up: Slack, Linear, Asana, Atlassian (Jira, Confluence), Notion, GitHub, PagerDuty, Datadog. Blank on purpose, connect them yourself: Google Calendar, Gmail.

Each connector signs in with your own account, and nothing connects until you do. [CONNECTORS.md](CONNECTORS.md) lists what each one needs.

## Good to know

- Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.
- Software suggests. People decide. Check what a skill produces before you use it.

## Credits and licence

Adapted by SMILE-FX P.A. from the `engineering` plugin in Anthropic's [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) (commit `da38ec1`), under the Apache License 2.0. SMILE-FX changed the plugin name and metadata, this README, the connector notes, and skill text that named the old plugin. The changes are listed in [MODIFICATIONS.md](../MODIFICATIONS.md). Licence: [LICENSE](LICENSE). Notices: [NOTICE](../NOTICE).

© 2026 SMILE-FX P.A. SMILE-FX® is a registered trademark of SMILE-FX P.A. SMILE-FX P.A. is not affiliated with, sponsored by or endorsed by Anthropic. Anthropic, Claude, Claude Code and Cowork are trademarks of Anthropic and are named here only to describe compatibility.

# SMILE-FX® Operations

> Documents processes, reviews vendors, plans capacity, tracks compliance tasks and writes status reports.

**Install id:** `sfx-operations` | **Version:** 1.0.0 | **Skills:** 9 | **Commands:** 0 | **Licence:** Apache-2.0

## Who it is for

Office and practice managers who own processes, vendors and the compliance calendar.

## Install

**Claude Code.** In a session:

```text
/plugin marketplace add wherewolf87/smile-fx-plugins
/plugin install sfx-operations@smile-fx-plugins
```

The install command opens the plugin panel so you can review it and pick a scope. From your shell, use `claude plugin marketplace add wherewolf87/smile-fx-plugins` and `claude plugin install sfx-operations@smile-fx-plugins`.

**Cowork.** Open **Customize**, then **Plugins**, then **Add marketplace**, and enter `wherewolf87/smile-fx-plugins`. Select **SMILE-FX Operations** and **Install**, then connect your tools on its **Connectors** tab. Plugins need a paid Claude plan.

Full steps: [install guide](../README.md#install).

## Try asking

- "Write an SOP for opening the office each morning."
- "Compare these two vendor quotes and list the risks."
- "Build a calendar of our annual license and permit renewals."

## Skills (9)

Claude uses a skill when your request matches it. You can also call one by name.

| Skill | What it does |
|---|---|
| `/sfx-operations:capacity-plan` | Plans workload and staffing capacity with a utilization forecast. |
| `/sfx-operations:change-request` | Writes a change request with impact analysis and a rollback plan. |
| `/sfx-operations:compliance-tracking` | Tracks compliance requirements and audit readiness. |
| `/sfx-operations:process-doc` | Documents a process as a flowchart, a RACI chart and an SOP. |
| `/sfx-operations:process-optimization` | Finds where a process slows down and proposes improvements. |
| `/sfx-operations:risk-assessment` | Identifies, rates and plans for operational risks. |
| `/sfx-operations:runbook` | Creates or updates a step-by-step runbook for a recurring task. |
| `/sfx-operations:status-report` | Writes a status report with measures, risks and action items. |
| `/sfx-operations:vendor-review` | Evaluates a vendor on cost and risk and gives a recommendation. |

## Connectors

Set up: Slack, Notion, Atlassian (Jira, Confluence), Asana. Blank on purpose, connect them yourself: Google Calendar, Gmail.

Each connector signs in with your own account, and nothing connects until you do. [CONNECTORS.md](CONNECTORS.md) lists what each one needs.

## Good to know

- Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.
- Software suggests. People decide. Check what a skill produces before you use it.

## Credits and licence

Adapted by SMILE-FX P.A. from the `operations` plugin in Anthropic's [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) (commit `da38ec1`), under the Apache License 2.0. SMILE-FX changed the plugin name and metadata, this README, the connector notes, and skill text that named the old plugin. The changes are listed in [MODIFICATIONS.md](../MODIFICATIONS.md). Licence: [LICENSE](LICENSE). Notices: [NOTICE](../NOTICE).

© 2026 SMILE-FX P.A. SMILE-FX® is a registered trademark of SMILE-FX P.A. SMILE-FX P.A. is not affiliated with, sponsored by or endorsed by Anthropic. Anthropic, Claude, Claude Code and Cowork are trademarks of Anthropic and are named here only to describe compatibility.

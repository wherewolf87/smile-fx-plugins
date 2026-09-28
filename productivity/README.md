# SMILE-FX® Productivity

> Keeps a task list and a working memory of your people, projects and shorthand, and pulls new tasks from your calendar, email and chat.

**Install id:** `sfx-productivity` | **Version:** 1.0.0 | **Skills:** 4 | **Commands:** 0 | **Licence:** Apache-2.0

## Who it is for

Anyone who wants a daily task list and a memory of people, projects and shorthand.

## Install

**Claude Code.** In a session:

```text
/plugin marketplace add wherewolf87/smile-fx-plugins
/plugin install sfx-productivity@smile-fx-plugins
```

The install command opens the plugin panel so you can review it and pick a scope. From your shell, use `claude plugin marketplace add wherewolf87/smile-fx-plugins` and `claude plugin install sfx-productivity@smile-fx-plugins`.

**Cowork.** Open **Customize**, then **Plugins**. Select **Add**, then **Add marketplace**, and enter `wherewolf87/smile-fx-plugins`. Select **SMILE-FX Productivity** and **Install**, then connect your tools on its **Connectors** tab. Plugins need a paid Claude plan.

Full steps: [install guide](../README.md#install).

## Try asking

- "Start."
- "What is on my plate today?"
- "Add a task: renew the business license by Friday."

## First run

Run `/sfx-productivity:start` once to create the task list and memory files, then `/sfx-productivity:update` to pull in new tasks.

## Skills (4)

Claude uses a skill when your request matches it. You can also call one by name.

| Skill | What it does |
|---|---|
| `memory-management` (automatic) | Keeps a working memory of your people, projects and shorthand so requests need less explaining. |
| `/sfx-productivity:start` | Sets up the task list and memory, and opens the dashboard. |
| `task-management` (automatic) | Keeps a shared task list in a TASKS.md file. |
| `/sfx-productivity:update` | Pulls in new tasks, triages stale ones and fills memory gaps from recent activity. |

Skills marked automatic have no slash command. Claude uses them when your request needs them.

## Connectors

Set up: Slack, Notion, Asana, Linear, Atlassian (Jira, Confluence), monday.com, ClickUp. Blank on purpose, connect them yourself: Google Calendar, Gmail.

Each connector signs in with your own account, and nothing connects until you do. [CONNECTORS.md](CONNECTORS.md) lists what each one needs.

## Good to know

- Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.
- Software suggests. People decide. Check what a skill produces before you use it.

## Credits and licence

Adapted by SMILE-FX P.A. from the `productivity` plugin in Anthropic's [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) (commit `da38ec1`), under the Apache License 2.0. SMILE-FX changed the plugin name and metadata, this README, the connector notes, and skill text that named the old plugin. The changes are listed in [MODIFICATIONS.md](../MODIFICATIONS.md). Licence: [LICENSE](LICENSE). Notices: [NOTICE](../NOTICE).

© 2026 SMILE-FX P.A. SMILE-FX® is a registered trademark of SMILE-FX P.A. SMILE-FX P.A. is not affiliated with, sponsored by or endorsed by Anthropic. Anthropic, Claude, Claude Code and Claude Cowork are trademarks of Anthropic, PBC. They are named here only to describe compatibility.

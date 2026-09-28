# SMILE-FX® Enterprise Search

> Searches your email, chat, documents and wikis in one request, and writes digests of what changed.

**Install id:** `sfx-enterprise-search` | **Version:** 1.0.0 | **Skills:** 5 | **Commands:** 0 | **Licence:** Apache-2.0

## Who it is for

Teams whose answers are spread across email, chat, documents and wikis.

## Install

**Claude Code.** In a session:

```text
/plugin marketplace add wherewolf87/smile-fx-plugins
/plugin install sfx-enterprise-search@smile-fx-plugins
```

The install command opens the plugin panel so you can review it and pick a scope. From your shell, use `claude plugin marketplace add wherewolf87/smile-fx-plugins` and `claude plugin install sfx-enterprise-search@smile-fx-plugins`.

**Cowork.** Open **Customize**, then **Plugins**, then **Add marketplace**, and enter `wherewolf87/smile-fx-plugins`. Select **SMILE-FX Enterprise Search** and **Install**, then connect your tools on its **Connectors** tab. Plugins need a paid Claude plan.

Full steps: [install guide](../README.md#install).

## Try asking

- "Find everything we decided about the new phone system."
- "Give me a weekly digest of what changed in Slack and Notion."
- "Which connected sources can you search right now?"

## Skills (5)

Claude uses a skill when your request matches it. You can also call one by name.

| Skill | What it does |
|---|---|
| `/sfx-enterprise-search:digest` | Writes a daily or weekly digest of activity across connected sources. |
| `/sfx-enterprise-search:knowledge-synthesis` | Combines results from several sources into one answer, with sources. |
| `/sfx-enterprise-search:search` | Searches all connected sources in one request. |
| `/sfx-enterprise-search:search-strategy` | Breaks a question into searches across several sources. |
| `/sfx-enterprise-search:source-management` | Detects connected sources, helps add new ones and sets their priority. |

## Connectors

Set up: Slack, Notion, Guru, Atlassian (Jira, Confluence), Asana. Blank on purpose, connect them yourself: Google Calendar, Gmail.

Each connector signs in with your own account, and nothing connects until you do. [CONNECTORS.md](CONNECTORS.md) lists what each one needs.

## Good to know

- Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.
- Software suggests. People decide. Check what a skill produces before you use it.

## Credits and licence

Adapted by SMILE-FX P.A. from the `enterprise-search` plugin in Anthropic's [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) (commit `da38ec1`), under the Apache License 2.0. SMILE-FX changed the plugin name and metadata, this README, the connector notes, and skill text that named the old plugin. The changes are listed in [MODIFICATIONS.md](../MODIFICATIONS.md). Licence: [LICENSE](LICENSE). Notices: [NOTICE](../NOTICE).

© 2026 SMILE-FX P.A. SMILE-FX® is a registered trademark of SMILE-FX P.A. SMILE-FX P.A. is not affiliated with, sponsored by or endorsed by Anthropic. Anthropic, Claude, Claude Code and Cowork are trademarks of Anthropic and are named here only to describe compatibility.

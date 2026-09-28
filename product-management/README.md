# SMILE-FX® Product Management

> Writes specs, plans roadmaps and sprints, synthesizes research, reviews metrics and drafts stakeholder updates.

**Install id:** `sfx-product-management` | **Version:** 1.0.0 | **Skills:** 8 | **Commands:** 1 | **Licence:** Apache-2.0

## Who it is for

Teams building a product, an app or a new service.

## Install

**Claude Code.** In a session:

```text
/plugin marketplace add wherewolf87/smile-fx-plugins
/plugin install sfx-product-management@smile-fx-plugins
```

The install command opens the plugin panel so you can review it and pick a scope. From your shell, use `claude plugin marketplace add wherewolf87/smile-fx-plugins` and `claude plugin install sfx-product-management@smile-fx-plugins`.

**Cowork.** Open **Customize**, then **Plugins**, then **Add marketplace**, and enter `wherewolf87/smile-fx-plugins`. Select **SMILE-FX Product Management** and **Install**, then connect your tools on its **Connectors** tab. Plugins need a paid Claude plan.

Full steps: [install guide](../README.md#install).

## Try asking

- "Write a one-page spec for an online new-client intake form."
- "Brainstorm ways to reduce missed appointments."
- "Draft a monthly update for the partners."

## Skills (8)

Claude uses a skill when your request matches it. You can also call one by name.

| Skill | What it does |
|---|---|
| `/sfx-product-management:competitive-brief` | Writes a competitive analysis for one or more competitors or a feature area. |
| `/sfx-product-management:metrics-review` | Reviews product measures with trends and actions. |
| `/sfx-product-management:product-brainstorming` | Explores ideas and problem spaces and challenges assumptions. |
| `/sfx-product-management:roadmap-update` | Creates, updates or reprioritizes a roadmap. |
| `/sfx-product-management:sprint-planning` | Scopes work, estimates capacity, sets goals and drafts a sprint plan. |
| `/sfx-product-management:stakeholder-update` | Writes an update for a given audience and cadence. |
| `/sfx-product-management:synthesize-research` | Turns interviews, surveys and feedback into structured insights. |
| `/sfx-product-management:write-spec` | Writes a feature spec or PRD from a problem statement. |

## Commands (1)

| Command | What it does |
|---|---|
| `/sfx-product-management:brainstorm` | Brainstorms an idea, problem or strategic question with you as a thinking partner. |

## Connectors

Set up: Slack, Linear, Asana, monday.com, ClickUp, Atlassian (Jira, Confluence), Notion, Figma, Amplitude (US), Amplitude (EU), Pendo, Intercom, Fireflies, Similarweb. Blank on purpose, connect them yourself: Google Calendar, Gmail.

Each connector signs in with your own account, and nothing connects until you do. [CONNECTORS.md](CONNECTORS.md) lists what each one needs.

## Good to know

- Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.
- Software suggests. People decide. Check what a skill produces before you use it.

## Credits and licence

Adapted by SMILE-FX P.A. from the `product-management` plugin in Anthropic's [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) (commit `da38ec1`), under the Apache License 2.0. SMILE-FX changed the plugin name and metadata, this README, the connector notes, and skill text that named the old plugin. The changes are listed in [MODIFICATIONS.md](../MODIFICATIONS.md). Licence: [LICENSE](LICENSE). Notices: [NOTICE](../NOTICE).

© 2026 SMILE-FX P.A. SMILE-FX® is a registered trademark of SMILE-FX P.A. SMILE-FX P.A. is not affiliated with, sponsored by or endorsed by Anthropic. Anthropic, Claude, Claude Code and Cowork are trademarks of Anthropic and are named here only to describe compatibility.

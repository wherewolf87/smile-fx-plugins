# SMILE-FX® Design

> Critiques designs, writes interface copy, reviews accessibility, synthesizes research and prepares developer handoff notes.

**Install id:** `sfx-design` | **Version:** 1.0.0 | **Skills:** 7 | **Commands:** 0 | **Licence:** Apache-2.0

## Who it is for

Teams that make websites, forms, print pieces or app screens.

## Install

**Claude Code.** In a session:

```text
/plugin marketplace add wherewolf87/smile-fx-plugins
/plugin install sfx-design@smile-fx-plugins
```

The install command opens the plugin panel so you can review it and pick a scope. From your shell, use `claude plugin marketplace add wherewolf87/smile-fx-plugins` and `claude plugin install sfx-design@smile-fx-plugins`.

**Cowork.** Open **Customize**, then **Plugins**. Select **Add**, then **Add marketplace**, and enter `wherewolf87/smile-fx-plugins`. Select **SMILE-FX Design** and **Install**, then connect your tools on its **Connectors** tab. Plugins need a paid Claude plan.

Full steps: [install guide](../README.md#install).

## Try asking

- "Critique this landing page screenshot."
- "Review our online form for accessibility issues."
- "Rewrite the error messages on our booking form."

## Skills (7)

Claude uses a skill when your request matches it. You can also call one by name.

| Skill | What it does |
|---|---|
| `/sfx-design:accessibility-review` | Runs a WCAG 2.1 AA accessibility audit on a design or page. |
| `/sfx-design:design-critique` | Gives structured feedback on usability, hierarchy and consistency. |
| `/sfx-design:design-handoff` | Writes developer handoff specs from a design. |
| `/sfx-design:design-system` | Audits, documents or extends your design system. |
| `/sfx-design:research-synthesis` | Turns user research into themes, insights and recommendations. |
| `/sfx-design:user-research` | Plans, runs and synthesizes user research. |
| `/sfx-design:ux-copy` | Writes or reviews interface copy: microcopy, error messages, empty states and calls to action. |

## Connectors

Set up: Slack, Figma, Linear, Asana, Atlassian (Jira, Confluence), Notion, Intercom. Blank on purpose, connect them yourself: Google Calendar, Gmail.

Each connector signs in with your own account, and nothing connects until you do. [CONNECTORS.md](CONNECTORS.md) lists what each one needs.

## Good to know

- Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.
- Software suggests. People decide. Check what a skill produces before you use it.

## Credits and licence

Adapted by SMILE-FX P.A. from the `design` plugin in Anthropic's [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) (commit `da38ec1`), under the Apache License 2.0. SMILE-FX changed the plugin name and metadata, this README, the connector notes, and punctuation in skill descriptions (long dashes replaced with commas or colons). The changes are listed in [MODIFICATIONS.md](../MODIFICATIONS.md). Licence: [LICENSE](LICENSE). Notices: [NOTICE](../NOTICE).

© 2026 SMILE-FX P.A. SMILE-FX® is a registered trademark of SMILE-FX P.A. SMILE-FX P.A. is not affiliated with, sponsored by or endorsed by Anthropic. Anthropic, Claude, Claude Code and Claude Cowork are trademarks of Anthropic, PBC. They are named here only to describe compatibility.

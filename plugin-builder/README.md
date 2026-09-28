# SMILE-FX® Plugin Builder

> Builds new plugins from scratch and customizes existing ones for your own tools, terms and workflows.

**Install id:** `sfx-plugin-builder` | **Version:** 1.0.0 | **Skills:** 2 | **Commands:** 0 | **Licence:** Apache-2.0

## Who it is for

Anyone who wants a plugin for their own routines, tools and vocabulary.

## Install

**Claude Code.** In a session:

```text
/plugin marketplace add wherewolf87/smile-fx-plugins
/plugin install sfx-plugin-builder@smile-fx-plugins
```

The install command opens the plugin panel so you can review it and pick a scope. From your shell, use `claude plugin marketplace add wherewolf87/smile-fx-plugins` and `claude plugin install sfx-plugin-builder@smile-fx-plugins`.

**Cowork.** Open **Customize**, then **Plugins**, then **Add marketplace**, and enter `wherewolf87/smile-fx-plugins`. Select **SMILE-FX Plugin Builder** and **Install**, then connect your tools on its **Connectors** tab. Plugins need a paid Claude plan.

Full steps: [install guide](../README.md#install).

## Try asking

- "Create a plugin for our front desk routines."
- "Customize SMILE-FX Marketing to use our CRM and brand terms."
- "What does a plugin folder need to contain?"

## First run

Both skills are written for Cowork: `create-plugin` delivers a `.plugin` file to the Cowork outputs folder, and `customize-plugin` edits plugins mounted in a Cowork session. In Claude Code they still guide you, but you save and test the files yourself with `claude plugin validate`.

## Skills (2)

Claude uses a skill when your request matches it. You can also call one by name.

| Skill | What it does |
|---|---|
| `/sfx-plugin-builder:create-plugin` | Guides you through building a new plugin from scratch. |
| `/sfx-plugin-builder:customize-plugin` | Adapts an existing plugin to your organization's tools and workflows. |

## Connectors

This plugin has no connectors. It works with what you share in the conversation.

## Good to know

- Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.
- Software suggests. People decide. Check what a skill produces before you use it.

## Credits and licence

Adapted by SMILE-FX P.A. from the `cowork-plugin-management` plugin in Anthropic's [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) (commit `da38ec1`), under the Apache License 2.0. SMILE-FX changed the plugin name and metadata, this README, the connector notes, and skill text that named the old plugin. The changes are listed in [MODIFICATIONS.md](../MODIFICATIONS.md). Licence: [LICENSE](LICENSE). Notices: [NOTICE](../NOTICE).

© 2026 SMILE-FX P.A. SMILE-FX® is a registered trademark of SMILE-FX P.A. SMILE-FX P.A. is not affiliated with, sponsored by or endorsed by Anthropic. Anthropic, Claude, Claude Code and Cowork are trademarks of Anthropic and are named here only to describe compatibility.

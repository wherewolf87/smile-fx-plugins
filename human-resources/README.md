# SMILE-FX® Human Resources

> Supports recruiting, onboarding, performance reviews, compensation analysis and policy questions.

**Install id:** `sfx-human-resources` | **Version:** 1.0.0 | **Skills:** 9 | **Commands:** 0 | **Licence:** Apache-2.0

## Who it is for

Owners and HR leads who hire, onboard and review a team.

## Install

**Claude Code.** In a session:

```text
/plugin marketplace add wherewolf87/smile-fx-plugins
/plugin install sfx-human-resources@smile-fx-plugins
```

The install command opens the plugin panel so you can review it and pick a scope. From your shell, use `claude plugin marketplace add wherewolf87/smile-fx-plugins` and `claude plugin install sfx-human-resources@smile-fx-plugins`.

**Cowork.** Open **Customize**, then **Plugins**. Select **Add**, then **Add marketplace**, and enter `wherewolf87/smile-fx-plugins`. Select **SMILE-FX Human Resources** and **Install**, then connect your tools on its **Connectors** tab. Plugins need a paid Claude plan.

Full steps: [install guide](../README.md#install).

## Try asking

- "Build a first-week onboarding plan for a new front desk hire."
- "Draft interview questions and a scorecard for a treatment coordinator role."
- "Explain our PTO policy in plain words."

## Skills (9)

Claude uses a skill when your request matches it. You can also call one by name.

| Skill | What it does |
|---|---|
| `/sfx-human-resources:comp-analysis` | Benchmarks pay, checks band placement and models equity. |
| `/sfx-human-resources:draft-offer` | Drafts an offer letter with pay details and terms. |
| `/sfx-human-resources:interview-prep` | Builds structured interview plans with questions and scorecards. |
| `/sfx-human-resources:onboarding` | Creates an onboarding checklist and a first-week plan. |
| `/sfx-human-resources:org-planning` | Plans headcount, team structure and reporting lines. |
| `/sfx-human-resources:people-report` | Builds headcount, attrition and team health reports. |
| `/sfx-human-resources:performance-review` | Structures a performance review with self-assessment and manager templates. |
| `/sfx-human-resources:policy-lookup` | Finds a company policy and explains it in plain words. |
| `/sfx-human-resources:recruiting-pipeline` | Tracks candidates through each recruiting stage. |

## Connectors

Set up: Slack, Notion, Atlassian (Jira, Confluence). Blank on purpose, connect them yourself: Google Calendar, Gmail.

Each connector signs in with your own account, and nothing connects until you do. [CONNECTORS.md](CONNECTORS.md) lists what each one needs.

## Good to know

- Employment law differs by state. Have offer letters and policy changes reviewed by a qualified professional.
- Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.
- Software suggests. People decide. Check what a skill produces before you use it.

## Credits and licence

Adapted by SMILE-FX P.A. from the `human-resources` plugin in Anthropic's [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) (commit `da38ec1`), under the Apache License 2.0. SMILE-FX changed the plugin name and metadata, this README, the connector notes, and punctuation in skill descriptions (long dashes replaced with commas or colons). The changes are listed in [MODIFICATIONS.md](../MODIFICATIONS.md). Licence: [LICENSE](LICENSE). Notices: [NOTICE](../NOTICE).

© 2026 SMILE-FX P.A. SMILE-FX® is a registered trademark of SMILE-FX P.A. SMILE-FX P.A. is not affiliated with, sponsored by or endorsed by Anthropic. Anthropic, Claude, Claude Code and Claude Cowork are trademarks of Anthropic, PBC. They are named here only to describe compatibility.

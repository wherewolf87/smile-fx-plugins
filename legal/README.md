# SMILE-FX® Legal

> Reviews contracts against your playbook, triages NDAs, checks compliance questions and drafts briefings for your counsel. It does not give legal advice.

**Install id:** `sfx-legal` | **Version:** 1.0.0 | **Skills:** 9 | **Commands:** 0 | **Licence:** Apache-2.0

## Who it is for

Owners and administrators who handle contracts and compliance questions before they go to counsel.

## Install

**Claude Code.** In a session:

```text
/plugin marketplace add wherewolf87/smile-fx-plugins
/plugin install sfx-legal@smile-fx-plugins
```

The install command opens the plugin panel so you can review it and pick a scope. From your shell, use `claude plugin marketplace add wherewolf87/smile-fx-plugins` and `claude plugin install sfx-legal@smile-fx-plugins`.

**Cowork.** Open **Customize**, then **Plugins**, then **Add marketplace**, and enter `wherewolf87/smile-fx-plugins`. Select **SMILE-FX Legal** and **Install**, then connect your tools on its **Connectors** tab. Plugins need a paid Claude plan.

Full steps: [install guide](../README.md#install).

## Try asking

- "Triage this vendor NDA."
- "Review this software agreement against our playbook and list the deviations."
- "What should I ask counsel before I sign this lease amendment?"

## First run

Write your playbook in a file named `legal.local.md`: your standard positions, acceptable ranges and what needs escalation, for NDAs and each clause type you care about. In Cowork, save it in a folder you share with Cowork. In Claude Code, save it in your project's `.claude/` folder. The contract, NDA and response skills look for it and ask for context when it is missing.

## Skills (9)

Claude uses a skill when your request matches it. You can also call one by name.

| Skill | What it does |
|---|---|
| `/sfx-legal:brief` | Writes briefings for legal work: daily summary, topic research or incident response. |
| `/sfx-legal:compliance-check` | Lists regulations, approvals and risk areas for a proposed action. |
| `/sfx-legal:legal-response` | Drafts replies to common legal questions from your templates, with escalation checks. |
| `/sfx-legal:legal-risk-assessment` | Rates legal risks by severity and likelihood, with escalation criteria. |
| `/sfx-legal:meeting-briefing` | Prepares briefings for meetings with legal relevance and tracks the actions. |
| `/sfx-legal:review-contract` | Reviews a contract against your negotiation playbook and drafts redlines. |
| `/sfx-legal:signature-request` | Runs a pre-signature checklist and routes a document for e-signature. |
| `/sfx-legal:triage-nda` | Sorts an incoming NDA into standard approval, counsel review or full review. |
| `/sfx-legal:vendor-check` | Checks existing agreements with a vendor across connected systems and flags deadlines. |

## Connectors

Set up: Slack, Box, Egnyte, Atlassian (Jira, Confluence), Docusign. Blank on purpose, connect them yourself: Google Calendar, Gmail.

Each connector signs in with your own account, and nothing connects until you do. [CONNECTORS.md](CONNECTORS.md) lists what each one needs.

These connectors can take actions such as payments, payroll, record changes or e-signature requests: Docusign. Read every action before you approve it.

## Good to know

- Not legal advice. Have a licensed attorney review anything that matters.
- Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.
- Software suggests. People decide. Check what a skill produces before you use it.

## Credits and licence

Adapted by SMILE-FX P.A. from the `legal` plugin in Anthropic's [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) (commit `da38ec1`), under the Apache License 2.0. SMILE-FX changed the plugin name and metadata, this README, the connector notes, and skill text that named the old plugin. The changes are listed in [MODIFICATIONS.md](../MODIFICATIONS.md). Licence: [LICENSE](LICENSE). Notices: [NOTICE](../NOTICE).

© 2026 SMILE-FX P.A. SMILE-FX® is a registered trademark of SMILE-FX P.A. SMILE-FX P.A. is not affiliated with, sponsored by or endorsed by Anthropic. Anthropic, Claude, Claude Code and Cowork are trademarks of Anthropic and are named here only to describe compatibility.

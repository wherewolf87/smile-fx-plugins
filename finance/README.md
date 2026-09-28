# SMILE-FX® Finance

> Prepares journal entries, reconciliations, financial statements and variance analysis, and supports month-end close and audit prep.

**Install id:** `sfx-finance` | **Version:** 1.0.0 | **Skills:** 8 | **Commands:** 0 | **Licence:** Apache-2.0

## Who it is for

Owners, bookkeepers and controllers who close the books and explain the numbers.

## Install

**Claude Code.** In a session:

```text
/plugin marketplace add wherewolf87/smile-fx-plugins
/plugin install sfx-finance@smile-fx-plugins
```

The install command opens the plugin panel so you can review it and pick a scope. From your shell, use `claude plugin marketplace add wherewolf87/smile-fx-plugins` and `claude plugin install sfx-finance@smile-fx-plugins`.

**Cowork.** Open **Customize**, then **Plugins**. Select **Add**, then **Add marketplace**, and enter `wherewolf87/smile-fx-plugins`. Select **SMILE-FX Finance** and **Install**, then connect your tools on its **Connectors** tab. Plugins need a paid Claude plan.

Full steps: [install guide](../README.md#install).

## Try asking

- "Reconcile this bank export against the ledger export."
- "Explain the variance between this month and last month."
- "Draft our month-end close checklist."

## Skills (8)

Claude uses a skill when your request matches it. You can also call one by name.

| Skill | What it does |
|---|---|
| `audit-support` (automatic) | Supports control testing, sample selection and audit documentation. |
| `close-management` (automatic) | Sequences and tracks month-end close tasks. |
| `/sfx-finance:financial-statements` | Builds the income statement, balance sheet and cash flow with period comparisons. |
| `/sfx-finance:journal-entry` | Prepares journal entries with debits, credits and support. |
| `journal-entry-prep` (automatic) | Prepares month-end journal entries with supporting documentation. |
| `/sfx-finance:reconciliation` | Reconciles ledger balances to subledgers, bank statements or other data. |
| `/sfx-finance:sox-testing` | Builds SOX sample selections, testing workpapers and control assessments. |
| `/sfx-finance:variance-analysis` | Breaks a variance into drivers with a written explanation. |

Skills marked automatic have no slash command. Claude uses them when your request needs them.

## Connectors

Set up: BigQuery, Slack. Blank on purpose, connect them yourself: Snowflake, Databricks, Google Calendar, Gmail.

Each connector signs in with your own account, and nothing connects until you do. [CONNECTORS.md](CONNECTORS.md) lists what each one needs.

## Good to know

- Outputs support your accountant. They are not tax or accounting advice.
- Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.
- Software suggests. People decide. Check what a skill produces before you use it.

## Credits and licence

Adapted by SMILE-FX P.A. from the `finance` plugin in Anthropic's [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) (commit `da38ec1`), under the Apache License 2.0. SMILE-FX changed the plugin name and metadata, this README, and the connector notes. The changes are listed in [MODIFICATIONS.md](../MODIFICATIONS.md). Licence: [LICENSE](LICENSE). Notices: [NOTICE](../NOTICE).

© 2026 SMILE-FX P.A. SMILE-FX® is a registered trademark of SMILE-FX P.A. SMILE-FX P.A. is not affiliated with, sponsored by or endorsed by Anthropic. Anthropic, Claude, Claude Code and Claude Cowork are trademarks of Anthropic, PBC. They are named here only to describe compatibility.

# SMILE-FX® Data

> Writes SQL, explores data sets, runs statistics, builds charts and dashboards, and checks an analysis before you share it.

**Install id:** `sfx-data` | **Version:** 1.0.0 | **Skills:** 10 | **Commands:** 0 | **Licence:** Apache-2.0

## Who it is for

Anyone who works with spreadsheets, exports or a data warehouse.

## Install

**Claude Code.** In a session:

```text
/plugin marketplace add wherewolf87/smile-fx-plugins
/plugin install sfx-data@smile-fx-plugins
```

The install command opens the plugin panel so you can review it and pick a scope. From your shell, use `claude plugin marketplace add wherewolf87/smile-fx-plugins` and `claude plugin install sfx-data@smile-fx-plugins`.

**Cowork.** Open **Customize**, then **Plugins**. Select **Add**, then **Add marketplace**, and enter `wherewolf87/smile-fx-plugins`. Select **SMILE-FX Data** and **Install**, then connect your tools on its **Connectors** tab. Plugins need a paid Claude plan.

Full steps: [install guide](../README.md#install).

## Try asking

- "Profile this monthly revenue CSV and flag data quality issues."
- "Write a SQL query for new customers by month."
- "Build a dashboard from this spreadsheet."

## Skills (10)

Claude uses a skill when your request matches it. You can also call one by name.

| Skill | What it does |
|---|---|
| `/sfx-data:analyze` | Answers data questions, from quick lookups to full analyses. |
| `/sfx-data:build-dashboard` | Builds an interactive HTML dashboard with charts, filters and tables. |
| `/sfx-data:create-viz` | Creates charts with Python. |
| `/sfx-data:data-context-extractor` | Builds a company-specific data skill from what your analysts know. |
| `data-visualization` (automatic) | Guidance and code for clear charts with matplotlib, seaborn or plotly. |
| `/sfx-data:explore-data` | Profiles a data set: shape, quality and patterns. |
| `sql-queries` (automatic) | Writes correct SQL across common warehouse dialects. |
| `statistical-analysis` (automatic) | Runs descriptive statistics, trends, outlier checks and hypothesis tests. |
| `/sfx-data:validate-data` | Checks an analysis for method, accuracy and bias before you share it. |
| `/sfx-data:write-query` | Writes SQL for your database dialect. |

Skills marked automatic have no slash command. Claude uses them when your request needs them.

## Connectors

Set up: BigQuery, Hex, Amplitude (US), Amplitude (EU), Atlassian (Jira, Confluence). Blank on purpose, connect them yourself: Snowflake, Databricks, Definite.

Each connector signs in with your own account, and nothing connects until you do. [CONNECTORS.md](CONNECTORS.md) lists what each one needs.

## Good to know

- Use de-identified or aggregate data unless your plan is covered by a signed BAA.
- Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.
- Software suggests. People decide. Check what a skill produces before you use it.

## Credits and licence

Adapted by SMILE-FX P.A. from the `data` plugin in Anthropic's [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) (commit `da38ec1`), under the Apache License 2.0. SMILE-FX changed the plugin name and metadata, this README, the connector notes, and the connector settings (Definite address left blank). The changes are listed in [MODIFICATIONS.md](../MODIFICATIONS.md). Licence: [LICENSE](LICENSE). Notices: [NOTICE](../NOTICE).

© 2026 SMILE-FX P.A. SMILE-FX® is a registered trademark of SMILE-FX P.A. SMILE-FX P.A. is not affiliated with, sponsored by or endorsed by Anthropic. Anthropic, Claude, Claude Code and Claude Cowork are trademarks of Anthropic, PBC. They are named here only to describe compatibility.

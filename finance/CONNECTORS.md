# Connectors

## How tool references work

Skills name a kind of tool instead of one product. In plugin files these appear as placeholders such as `~~chat` or `~~CRM`. Any connector in that category works. The plugin's `.mcp.json` sets up the connectors listed under setup notes, and you can connect a different tool in the same category instead.

## Connectors for this plugin

| Category | Placeholder | Set up in this plugin | Other options |
|----------|-------------|-----------------|---------------|
| Data warehouse | `~~data warehouse` | Snowflake (blank address), Databricks (blank address), BigQuery | Redshift, PostgreSQL |
| Email | `~~email` | None | Microsoft 365 |
| Office suite | `~~office suite` | None | Microsoft 365 |
| Chat | `~~chat` | Slack | Microsoft Teams |
| ERP / Accounting | `~~erp` | None | NetSuite, SAP, QuickBooks, Xero |
| Analytics / BI | `~~analytics` | None | Tableau, Looker, Power BI |

"Set up in this plugin" lists the connectors in this plugin's `.mcp.json`. "(blank address)" marks a placeholder you connect yourself.

## Setup notes

Every connector below signs in with your own account for that service. Nothing connects until you sign in, and installing the plugin does not sign you in to anything. In Cowork, open the plugin's **Connectors** tab. In Claude Code, run `/mcp`.

| Connector | Address | What you need | Check on September 27, 2026 | Notes |
|---|---|---|---|---|
| Snowflake | (blank) | Your own Snowflake account and its MCP address | Placeholder | Blank on purpose. Every account has its own MCP address. Ask your data admin for it, then add the server in your app. |
| Databricks | (blank) | Your own Databricks account and its MCP address | Placeholder | Blank on purpose. Every account has its own MCP address. Ask your data admin for it, then add the server in your app. |
| BigQuery | `https://bigquery.googleapis.com/mcp` | Your own Google Cloud project with BigQuery | Reachable (200) | Signs in with Google. If Claude Code reports that the server does not support dynamic client registration, create an OAuth client in your own Google Cloud project and add the server with `--client-id`. |
| Slack | `https://mcp.slack.com/mcp` | Your own Slack workspace, with admin approval | Sign-in required (401) | Uses the sign-in app Slack publishes for Claude Code. A workspace admin must approve the Slack MCP app. |
| Google Calendar | (blank) | Your own Google Calendar account | Placeholder | Blank on purpose, so it shows as "not configured" instead of an error. Connect Google Calendar from your Claude connector settings, or add Google's MCP server yourself. The skills use any calendar tool you connect. |
| Gmail | (blank) | Your own Gmail account | Placeholder | Blank on purpose, so it shows as "not configured" instead of an error. Connect Gmail from your Claude connector settings, or add Google's MCP server yourself. The skills use any email tool you connect. |

The check column is an anonymous request sent on September 27, 2026 with no account: it shows whether the address answered and asked for sign-in, not whether your account works. The full list for all plugins is in [CONNECTORS.md](../CONNECTORS.md) at the repository root.

Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.

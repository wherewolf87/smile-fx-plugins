<!-- Modified by SMILE-FX P.A. in 2026 for SMILE-FX Plugins. MODIFICATIONS.md at the repository root lists what changed in this file. Original: https://github.com/anthropics/knowledge-work-plugins (Apache License 2.0). -->

# Connectors

## How tool references work

Skills name a kind of tool instead of one product. In plugin files these appear as placeholders such as `~~chat` or `~~CRM`. Any connector in that category works. The plugin's `.mcp.json` sets up the connectors listed under setup notes, and you can connect a different tool in the same category instead.

## Connectors for this plugin

| Category | Placeholder | Set up in this plugin | Other options |
|----------|-------------|-----------------|---------------|
| Data warehouse | `~~data warehouse` | Snowflake (blank address), Databricks (blank address), BigQuery, Definite (blank address) | Redshift, PostgreSQL, MySQL |
| Notebook | `~~notebook` | Hex | Jupyter, Deepnote, Observable |
| Product analytics | `~~product analytics` | Amplitude | Mixpanel, Heap |
| Project tracker | `~~project tracker` | Atlassian (Jira/Confluence) | Linear, Asana |

"Set up in this plugin" lists the connectors in this plugin's `.mcp.json`. "(blank address)" marks a placeholder you connect yourself.

## Setup notes

Every connector below signs in with your own account for that service. Nothing connects until you sign in, and installing the plugin does not sign you in to anything. In Cowork, open the plugin's **Connectors** tab. In Claude Code, run `/mcp`.

| Connector | Address | What you need | Check on September 27, 2026 | Notes |
|---|---|---|---|---|
| Snowflake | (blank) | Your own Snowflake account and its MCP address | Placeholder | Blank on purpose. Every account has its own MCP address. Ask your data admin for it, then add the server in your app. |
| Databricks | (blank) | Your own Databricks account and its MCP address | Placeholder | Blank on purpose. Every account has its own MCP address. Ask your data admin for it, then add the server in your app. |
| BigQuery | `https://bigquery.googleapis.com/mcp` | Your own Google Cloud project with BigQuery | Reachable (200) | Signs in with Google. If Claude Code reports that the server does not support dynamic client registration, create an OAuth client in your own Google Cloud project and add the server with `--client-id`. |
| Hex | `https://app.hex.tech/mcp` | Your own Hex account | Sign-in required (401) | None. |
| Amplitude (US) | `https://mcp.amplitude.com/mcp` | Your own Amplitude account | Sign-in required (401) | None. |
| Amplitude (EU) | `https://mcp.eu.amplitude.com/mcp` | Your own Amplitude account | Sign-in required (401) | For Amplitude projects hosted in the EU. |
| Atlassian (Jira, Confluence) | `https://mcp.atlassian.com/v1/mcp` | Your own Atlassian account | Sign-in required (401) | None. |
| Definite | (blank) | Your own Definite deployment address | Placeholder | Blank on purpose. The upstream address `https://api.definite.app/v3/mcp/http` returned HTTP 404 on September 27, 2026, and Definite now documents MCP at your own deployment address. |

The check column is an anonymous request sent on September 27, 2026 with no account: it shows whether the address answered and asked for sign-in, not whether your account works. The full list for all plugins is in [CONNECTORS.md](../CONNECTORS.md) at the repository root.

Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.

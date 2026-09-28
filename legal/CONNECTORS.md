<!-- Modified by SMILE-FX P.A. in 2026 for SMILE-FX Plugins. MODIFICATIONS.md at the repository root lists what changed in this file. Original: https://github.com/anthropics/knowledge-work-plugins (Apache License 2.0). -->

# Connectors

## How tool references work

Skills name a kind of tool instead of one product. In plugin files these appear as placeholders such as `~~chat` or `~~CRM`. Any connector in that category works. The plugin's `.mcp.json` sets up the connectors listed under setup notes, and you can connect a different tool in the same category instead.

## Connectors for this plugin

| Category | Placeholder | Set up in this plugin | Other options |
|----------|-------------|-----------------|---------------|
| Calendar | `~~calendar` | Google Calendar (blank address) | Microsoft 365 |
| Chat | `~~chat` | Slack | Microsoft Teams |
| Cloud storage | `~~cloud storage` | Box, Egnyte | Dropbox, SharePoint, Google Drive |
| CLM | `~~CLM` | None | Ironclad, Agiloft |
| CRM | `~~CRM` | None | Salesforce, HubSpot |
| Email | `~~email` | Gmail (blank address) | Microsoft 365 |
| E-signature | `~~e-signature` | DocuSign | Adobe Sign |
| Office suite | `~~office suite` | None | Microsoft 365, Google Workspace |
| Project tracker | `~~project tracker` | Atlassian (Jira/Confluence) | Linear, Asana |

"Set up in this plugin" lists the connectors in this plugin's `.mcp.json`. "(blank address)" marks a placeholder you connect yourself.

## Setup notes

Every connector below signs in with your own account for that service. Nothing connects until you sign in, and installing the plugin does not sign you in to anything. In Cowork, open the plugin's **Connectors** tab. In Claude Code, run `/mcp`.

These connectors can take actions such as payments, payroll, record changes or e-signature requests: Docusign. Read every action before you approve it.

| Connector | Address | What you need | Check on September 27, 2026 | Notes |
|---|---|---|---|---|
| Slack | `https://mcp.slack.com/mcp` | Your own Slack workspace, with admin approval | Sign-in required (401) | Uses the sign-in app Slack publishes for Claude Code. A workspace admin must approve the Slack MCP app. |
| Box | `https://mcp.box.com` | Your own Box account | Sign-in required (401) | None. |
| Egnyte | `https://mcp-server.egnyte.com/mcp` | Your own Egnyte account | Sign-in required (401) | None. |
| Atlassian (Jira, Confluence) | `https://mcp.atlassian.com/v1/mcp` | Your own Atlassian account | Sign-in required (401) | None. |
| Docusign | `https://mcp.docusign.com/mcp` | Your own Docusign account | Refused anonymous check (403) | The server refused an anonymous check on September 27, 2026, so it could not be verified without an account. Its tools may include sending documents for signature. Read every action before you approve it. |
| Google Calendar | (blank) | Your own Google Calendar account | Placeholder | Blank on purpose, so it shows as "not configured" instead of an error. Connect Google Calendar from your Claude connector settings, or add Google's MCP server yourself. The skills use any calendar tool you connect. |
| Gmail | (blank) | Your own Gmail account | Placeholder | Blank on purpose, so it shows as "not configured" instead of an error. Connect Gmail from your Claude connector settings, or add Google's MCP server yourself. The skills use any email tool you connect. |

The check column is an anonymous request sent on September 27, 2026 with no account: it shows whether the address answered and asked for sign-in, not whether your account works. The full list for all plugins is in [CONNECTORS.md](../CONNECTORS.md) at the repository root.

Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.

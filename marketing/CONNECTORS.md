<!-- Modified by SMILE-FX P.A. in 2026 for SMILE-FX Plugins. MODIFICATIONS.md at the repository root lists what changed in this file. Original: https://github.com/anthropics/knowledge-work-plugins (Apache License 2.0). -->

# Connectors

## How tool references work

Skills name a kind of tool instead of one product. In plugin files these appear as placeholders such as `~~chat` or `~~CRM`. Any connector in that category works. The plugin's `.mcp.json` sets up the connectors listed under setup notes, and you can connect a different tool in the same category instead.

## Connectors for this plugin

| Category | Placeholder | Set up in this plugin | Other options |
|----------|-------------|-----------------|---------------|
| Chat | `~~chat` | Slack | Microsoft Teams |
| Design | `~~design` | Canva, Figma | Adobe Creative Cloud |
| Marketing automation | `~~marketing automation` | HubSpot | Marketo, Pardot, Mailchimp |
| Product analytics | `~~product analytics` | Amplitude | Mixpanel, Google Analytics |
| Knowledge base | `~~knowledge base` | Notion | Confluence, Guru |
| SEO | `~~SEO` | Ahrefs, Similarweb | Semrush, Moz |
| Email marketing | `~~email marketing` | Klaviyo | Mailchimp, Brevo, Customer.io |
| Marketing analytics | `~~marketing analytics` | Supermetrics | Google Analytics, Mailchimp, Semrush |

"Set up in this plugin" lists the connectors in this plugin's `.mcp.json`. "(blank address)" marks a placeholder you connect yourself.

## Setup notes

Every connector below signs in with your own account for that service. Nothing connects until you sign in, and installing the plugin does not sign you in to anything. In Cowork, open the plugin's **Connectors** tab. In Claude Code, run `/mcp`.

| Connector | Address | What you need | Check on September 27, 2026 | Notes |
|---|---|---|---|---|
| Slack | `https://mcp.slack.com/mcp` | Your own Slack workspace, with admin approval | Sign-in required (401) | Uses the sign-in app Slack publishes for Claude Code. A workspace admin must approve the Slack MCP app. |
| Canva | `https://mcp.canva.com/mcp` | Your own Canva account | Sign-in required (401) | None. |
| Figma | `https://mcp.figma.com/mcp` | Your own Figma account | Sign-in required (401) | None. |
| HubSpot | `https://mcp.hubspot.com/anthropic` | Your own HubSpot account | Sign-in required (401) | The vendor runs this address for Claude apps. |
| Amplitude (US) | `https://mcp.amplitude.com/mcp` | Your own Amplitude account | Sign-in required (401) | None. |
| Amplitude (EU) | `https://mcp.eu.amplitude.com/mcp` | Your own Amplitude account | Sign-in required (401) | For Amplitude projects hosted in the EU. |
| Notion | `https://mcp.notion.com/mcp` | Your own Notion account | Sign-in required (401) | None. |
| Ahrefs | `https://api.ahrefs.com/mcp/mcp` | Your own Ahrefs account | Sign-in required (401) | None. |
| Similarweb | `https://mcp.similarweb.com` | Your own Similarweb account | Sign-in required (401) | None. |
| Klaviyo | `https://mcp.klaviyo.com/mcp` | Your own Klaviyo account | Sign-in required (401) | None. |
| Supermetrics | `https://mcp.supermetrics.com/mcp` | Your own Supermetrics account | Sign-in required (401) | None. |
| Google Calendar | (blank) | Your own Google Calendar account | Placeholder | Blank on purpose, so it shows as "not configured" instead of an error. Connect Google Calendar from your Claude connector settings, or add Google's MCP server yourself. The skills use any calendar tool you connect. |
| Gmail | (blank) | Your own Gmail account | Placeholder | Blank on purpose, so it shows as "not configured" instead of an error. Connect Gmail from your Claude connector settings, or add Google's MCP server yourself. The skills use any email tool you connect. |

The check column is an anonymous request sent on September 27, 2026 with no account: it shows whether the address answered and asked for sign-in, not whether your account works. The full list for all plugins is in [CONNECTORS.md](../CONNECTORS.md) at the repository root.

Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.

# Connectors

## How tool references work

The plugin's `.mcp.json` sets up the connectors listed under setup notes. You can connect a different tool in the same category instead.

The skills in this plugin name the category in plain words ("the CRM", "email", "the calendar", "call transcripts") instead of `~~` placeholders. Either way, any connector in that category works. The placeholder column maps each category to the names used across plugins. Every skill also works with nothing connected: upload an export or paste notes, and the skill works from that.

## Connectors for this plugin

| Category | Placeholder | Set up in this plugin | Other options |
|----------|-------------|-----------------|---------------|
| CRM | `~~CRM` | HubSpot, Salesforce, Close, Monday | Pipedrive, Attio, Zoho CRM, Copper |
| Email | `~~email` | Gmail (blank address), Microsoft 365 (Outlook) | None |
| Calendar | `~~calendar` | Google Calendar (blank address), Calendly, Microsoft 365 (Outlook) | None |
| Chat | `~~chat` | Slack, Microsoft 365 (Teams) | None |
| Docs and knowledge base | `~~knowledge base` | Google Drive (blank address), Notion, Atlassian (Confluence), Microsoft 365 (SharePoint) | Box, Dropbox, Guru |
| Conversation intelligence | `~~conversation intelligence` | Gong, Fireflies, Zoom, Otter.ai | Granola, Fathom, Chorus |
| Data enrichment | `~~data enrichment` | Clay, ZoomInfo, Apollo, Lusha, Crunchbase | Clearbit |
| Sales engagement | `~~sales engagement` | Outreach, Apollo | Salesloft |
| Competitive intelligence | `~~competitive intelligence` | Similarweb | Crayon, Klue |
| Project tracker | `~~project tracker` | Atlassian (Jira) | Linear, Asana |

"Set up in this plugin" lists the connectors in this plugin's `.mcp.json`. "(blank address)" marks a placeholder you connect yourself.

## Setup notes

Every connector below signs in with your own account for that service. Nothing connects until you sign in, and installing the plugin does not sign you in to anything. In Cowork, open the plugin's **Connectors** tab. In Claude Code, run `/mcp`.

| Connector | Address | What you need | Check on September 27, 2026 | Notes |
|---|---|---|---|---|
| Slack | `https://mcp.slack.com/mcp` | Your own Slack workspace, with admin approval | Sign-in required (401) | Uses the sign-in app Slack publishes for Claude Code. A workspace admin must approve the Slack MCP app. |
| HubSpot | `https://mcp.hubspot.com/anthropic` | Your own HubSpot account | Sign-in required (401) | The vendor runs this address for Claude apps. |
| Salesforce | `https://api.salesforce.com/platform/mcp/v1/platform/headless-360` | Your own Salesforce org, with admin setup | Account required (401) | An admin enables this connector in Claude and sets up your org's Salesforce app before people can sign in. |
| Close | `https://mcp.close.com/mcp` | Your own Close account | Sign-in required (401) | None. |
| monday.com | `https://mcp.monday.com/mcp` | Your own monday.com account | Sign-in required (401) | None. |
| Clay | `https://api.clay.com/v3/mcp` | Your own Clay account | Sign-in required (401) | None. |
| ZoomInfo | `https://mcp.zoominfo.com/mcp` | Your own ZoomInfo account | Sign-in required (401) | None. |
| Notion | `https://mcp.notion.com/mcp` | Your own Notion account | Sign-in required (401) | None. |
| Atlassian (Jira, Confluence) | `https://mcp.atlassian.com/v1/mcp` | Your own Atlassian account | Sign-in required (401) | None. |
| Fireflies | `https://api.fireflies.ai/mcp` | Your own Fireflies account | Sign-in required (401) | None. |
| Apollo | `https://mcp.apollo.io/mcp` | Your own Apollo account | Sign-in required (401) | None. |
| Outreach | `https://api.outreach.io/mcp/` | Your own Outreach account | Sign-in required (401) | None. |
| Google Calendar | (blank) | Your own Google Calendar account | Placeholder | Blank on purpose, so it shows as "not configured" instead of an error. Connect Google Calendar from your Claude connector settings, or add Google's MCP server yourself. The skills use any calendar tool you connect. |
| Gmail | (blank) | Your own Gmail account | Placeholder | Blank on purpose, so it shows as "not configured" instead of an error. Connect Gmail from your Claude connector settings, or add Google's MCP server yourself. The skills use any email tool you connect. |
| Microsoft 365 | `https://microsoft365.mcp.claude.com/mcp` | Your own Microsoft 365 work account, with admin setup | Sign-in required (401) | An admin enables this connector in Claude before people can sign in. The address is hosted by Anthropic for Claude apps and was not verified outside them. |
| Similarweb | `https://mcp.similarweb.com/mcp` | Your own Similarweb account | Sign-in required (401) | None. |
| Google Drive | (blank) | Your own Google Drive account | Placeholder | Blank on purpose, so it shows as "not configured" instead of an error. Connect Google Drive from your Claude connector settings, or add Google's MCP server yourself. The skills use any file storage tool you connect. |
| Gong | `https://mcp.gong.io/mcp` | Your own Gong account | Sign-in required (401) | None. |
| Zoom | `https://mcp.zoom.us/mcp/zoom/streamable` | Your own Zoom account | Sign-in required (401) | None. |
| Otter.ai | `https://mcp.otter.ai/mcp` | Your own Otter.ai account | Sign-in required (401) | None. |
| Calendly | `https://mcp.calendly.com/` | Your own Calendly account | Sign-in required (401) | None. |
| Lusha | `https://mcp.lusha.com/mcp/claude` | Your own Lusha account | Sign-in required (401) | The vendor runs this address for Claude apps. |
| Crunchbase | `https://mcp.crunchbase.com/` | Your own Crunchbase account | Sign-in required (401) | None. |

The check column is an anonymous request sent on September 27, 2026 with no account: it shows whether the address answered and asked for sign-in, not whether your account works. The full list for all plugins is in [CONNECTORS.md](../CONNECTORS.md) at the repository root.

Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.

## Permissions

What a connector may do is set on the connector itself: allow, ask or block, tool by tool. The skills stay within those settings.

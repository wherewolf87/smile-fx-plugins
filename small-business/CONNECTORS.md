# Connectors

## How tool references work

The plugin's `.mcp.json` sets up the connectors listed under setup notes. You can connect a different tool in the same category instead.

## Connectors for this plugin

This plugin's skills ask which tools you use and call the connector for each one. Connectors in the same category are treated as equals: a ledger is a ledger, a CRM is a CRM. The rule is in `shared/connector-neutrality.md`.

## Setup notes

Every connector below signs in with your own account for that service. Nothing connects until you sign in, and installing the plugin does not sign you in to anything. In Cowork, open the plugin's **Connectors** tab. In Claude Code, run `/mcp`.

These connectors can take actions such as payments, payroll, record changes or e-signature requests: Airwallex, Docusign, Expensify, Gusto, QuickBooks, MYOB, PayPal, Ramp, Shopify, Square, Stripe, Xero, Zoho Books. Read every action before you approve it.

| Connector | Address | What you need | Check on September 27, 2026 | Notes |
|---|---|---|---|---|
| Airwallex | `https://mcp.airwallex.com/mcp` | Your own Airwallex account | Sign-in required (401) | Its tools may include transfers and bill payments. Read every action before you approve it. |
| Apollo | `https://mcp.apollo.io/mcp` | Your own Apollo account | Sign-in required (401) | None. |
| Atlassian (Jira, Confluence) | `https://mcp.atlassian.com/v1/mcp` | Your own Atlassian account | Sign-in required (401) | None. |
| Canva | `https://mcp.canva.com/mcp` | Your own Canva account | Sign-in required (401) | None. |
| Clay | `https://api.clay.com/v3/mcp` | Your own Clay account | Sign-in required (401) | None. |
| Docusign | `https://mcp.docusign.com/mcp` | Your own Docusign account | Refused anonymous check (403) | The server refused an anonymous check on September 27, 2026, so it could not be verified without an account. Its tools may include sending documents for signature. Read every action before you approve it. |
| Emergent | `https://mcp.emergent.sh` | Your own Emergent account | Sign-in required (401) | None. |
| Expensify | `https://www.expensify.com/mcp` | Your own Expensify account | Reachable, redirects (308) | Its tools may include expense reports and approvals. Read every action before you approve it. |
| Gmail | `https://gmailmcp.googleapis.com/mcp/v1` | Your own Gmail account | Reachable (200) | Signs in with Google. If Claude Code reports that the server does not support dynamic client registration, create an OAuth client in your own Google Cloud project and add the server with `--client-id`. |
| Google Calendar | `https://calendarmcp.googleapis.com/mcp/v1` | Your own Google Calendar account | Reachable (200) | Signs in with Google. If Claude Code reports that the server does not support dynamic client registration, create an OAuth client in your own Google Cloud project and add the server with `--client-id`. |
| Google Drive | `https://drivemcp.googleapis.com/mcp/v1` | Your own Google Drive account | Reachable (200) | Signs in with Google. If Claude Code reports that the server does not support dynamic client registration, create an OAuth client in your own Google Cloud project and add the server with `--client-id`. |
| Gusto | `https://mcp.api.gusto.com/anthropic` | Your own Gusto account | Sign-in required (401) | The vendor runs this address for Claude apps. Its tools may include payroll changes. Read every action before you approve it. |
| HubSpot | `https://mcp.hubspot.com/anthropic` | Your own HubSpot account | Sign-in required (401) | The vendor runs this address for Claude apps. |
| Mailchimp | `https://ai-inc.mailchimp.com/claude/mcp/v2` | Your own Mailchimp account | Refused anonymous check (403) | The vendor runs this address for Claude apps. The server refused an anonymous check on September 27, 2026, so it could not be verified without an account. |
| QuickBooks | `https://ai-inc.quickbooks.intuit.com/v1/mcp` | Your own QuickBooks account | Refused anonymous check (403) | The server refused an anonymous check on September 27, 2026, so it could not be verified without an account. Its tools may include creating and changing accounting records. Read every action before you approve it. |
| monday.com | `https://mcp.monday.com/mcp` | Your own monday.com account | Sign-in required (401) | None. |
| MYOB | `https://mcp.myob.com/mcp` | Your own MYOB account | Sign-in required (401) | Its tools may include creating and changing accounting records. Read every action before you approve it. |
| Notion | `https://mcp.notion.com/mcp` | Your own Notion account | Sign-in required (401) | None. |
| PayPal | `https://mcp.paypal.com/mcp` | Your own PayPal account | Sign-in required (401) | Its tools may include payments, refunds and invoices. Read every action before you approve it. |
| Ramp | `https://mcp.ramp.com/mcp` | Your own Ramp account | Sign-in required (401) | Its tools may include cards, bills and payments. Read every action before you approve it. |
| RingCentral team chat | `https://mcp.labs.ringcentral.com/ringex/v1.1.0/team-chat` | Your own RingCentral team chat account | Sign-in required (401) | None. |
| Shopify | `https://setup.shopify.com/mcp` | Your own Shopify account | Reachable (200) | Answers without sign-in for store setup and sample catalogs. Your own store data needs your Shopify sign-in. Its tools may include changes to products, prices, inventory and orders. Read every action before you approve it. |
| Slack | `https://mcp.slack.com/mcp` | Your own Slack workspace, with admin approval | Sign-in required (401) | Uses the sign-in app Slack publishes for Claude Code. A workspace admin must approve the Slack MCP app. |
| Square | `https://mcp.squareup.com/mcp` | Your own Square account | Sign-in required (401) | Its tools may include payments, refunds and invoices. Read every action before you approve it. |
| Stripe | `https://mcp.stripe.com` | Your own Stripe account | Sign-in required (401) | Its tools may include payments, refunds and invoices. Read every action before you approve it. |
| TikTok Ads | `https://business-api.tiktok.com/open_mcp/tt-ads-mcp-layer` | Your own TikTok Ads account | Sign-in required (401) | None. |
| Trello | `https://mcp.trello.com/v1` | Your own Trello account | Sign-in required (401) | None. |
| Wix | `https://mcp.wix.com/mcp` | Your own Wix account | Sign-in required (401) | None. |
| Xero | `https://mcp.xero.com/mcp` | Your own Xero account | Sign-in required (401) | Its tools may include creating and changing accounting records. Read every action before you approve it. |
| Zapier | `https://mcp.zapier.com/api/v1/connect` | Your own Zapier account | Sign-in required (401) | None. |
| Zoho Books | `https://claude-zohobooks.zohomcp.com/mcp/message` | Your own Zoho Books account | Sign-in required (401) | The vendor runs this address for Claude apps. Its tools may include creating and changing accounting records. Read every action before you approve it. |
| Zoho CRM | `https://claude-zohocrm.zohomcp.com/mcp/message` | Your own Zoho CRM account | Sign-in required (401) | The vendor runs this address for Claude apps. |
| Zoho Desk | `https://claude-zohodesk.zohomcp.com/mcp/message` | Your own Zoho Desk account | Sign-in required (401) | The vendor runs this address for Claude apps. |
| Zoho Projects | `https://claude-zohoprojects.zohomcp.com/mcp/message` | Your own Zoho Projects account | Sign-in required (401) | The vendor runs this address for Claude apps. |
| Zoom | `https://mcp.zoom.us/mcp/zoom/streamable` | Your own Zoom account | Sign-in required (401) | None. |

The check column is an anonymous request sent on September 27, 2026 with no account: it shows whether the address answered and asked for sign-in, not whether your account works. The full list for all plugins is in [CONNECTORS.md](../CONNECTORS.md) at the repository root.

Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.

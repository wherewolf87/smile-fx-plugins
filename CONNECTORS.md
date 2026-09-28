# Connectors

Connectors are MCP servers that let Claude read from and act in the tools you already use. Each SMILE-FX® plugin ships with a list of them in its `.mcp.json`. This page lists every one, what it needs, and what we saw when we checked it.

## Before you connect anything

- **Every connector needs your own account** with that service. Nothing connects until you sign in, and installing a plugin does not sign you in to anything.
- **Placeholders are blank on purpose.** Six connectors have no address in 30 places across the plugins. Claude Code shows them as "not configured" and does not try to connect, as its documentation describes. Connect those tools yourself (see the notes).
- **Some connectors can take actions,** such as payments, payroll, record changes or e-signature requests. Your app's permission settings decide whether each tool runs straight away or asks you first. Keep tools that send, pay or change records on ask, and read every action before you approve it.
- **Patient health information:** Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.

## How to connect

- **Cowork:** open the plugin, then its **Connectors** tab, then connect each tool you use.
- **Claude Code:** run `/mcp`, pick the server and sign in. For a placeholder, add your own server with `claude mcp add`.

## All connectors

The check column is an anonymous MCP request sent on September 27, 2026 with no account. "Sign-in required (401)" means the address answered and asked for sign-in, which is the expected result. It does not test your account.

| Connector | Address | Plugins | What you need | Check on September 27, 2026 | Notes |
|---|---|---|---|---|---|
| Ahrefs | `https://api.ahrefs.com/mcp/mcp` | `sfx-marketing` | Your own Ahrefs account | Sign-in required (401) | None. |
| Airwallex | `https://mcp.airwallex.com/mcp` | `sfx-small-business` | Your own Airwallex account | Sign-in required (401) | Its tools may include transfers and bill payments. Read every action before you approve it. |
| Amplitude (EU) | `https://mcp.eu.amplitude.com/mcp` | `sfx-marketing`, `sfx-data`, `sfx-product-management` | Your own Amplitude account | Sign-in required (401) | For Amplitude projects hosted in the EU. |
| Amplitude (US) | `https://mcp.amplitude.com/mcp` | `sfx-marketing`, `sfx-data`, `sfx-product-management` | Your own Amplitude account | Sign-in required (401) | None. |
| Apollo | `https://mcp.apollo.io/mcp` | `sfx-small-business`, `sfx-sales` | Your own Apollo account | Sign-in required (401) | None. |
| Asana | `https://mcp.asana.com/v2/mcp` | `sfx-operations`, `sfx-productivity`, `sfx-design`, `sfx-enterprise-search`, `sfx-product-management`, `sfx-engineering` | Your own Asana account | Sign-in required (401) | None. |
| Atlassian (Jira, Confluence) | `https://mcp.atlassian.com/v1/mcp` | `sfx-small-business`, `sfx-sales`, `sfx-customer-support`, `sfx-operations`, `sfx-human-resources`, `sfx-productivity`, `sfx-legal`, `sfx-data`, `sfx-design`, `sfx-enterprise-search`, `sfx-product-management`, `sfx-engineering` | Your own Atlassian account | Sign-in required (401) | None. |
| BigQuery | `https://bigquery.googleapis.com/mcp` | `sfx-finance`, `sfx-data` | Your own Google Cloud project with BigQuery | Reachable (200) | Signs in with Google. If Claude Code reports that the server does not support dynamic client registration, create an OAuth client in your own Google Cloud project and add the server with `--client-id`. |
| Box | `https://mcp.box.com` | `sfx-legal` | Your own Box account | Sign-in required (401) | None. |
| Calendly | `https://mcp.calendly.com/` | `sfx-sales` | Your own Calendly account | Sign-in required (401) | None. |
| Canva | `https://mcp.canva.com/mcp` | `sfx-small-business`, `sfx-marketing` | Your own Canva account | Sign-in required (401) | None. |
| Clay | `https://api.clay.com/v3/mcp` | `sfx-small-business`, `sfx-sales` | Your own Clay account | Sign-in required (401) | None. |
| ClickUp | `https://mcp.clickup.com/mcp` | `sfx-productivity`, `sfx-product-management` | Your own ClickUp account | Sign-in required (401) | None. |
| Close | `https://mcp.close.com/mcp` | `sfx-sales` | Your own Close account | Sign-in required (401) | None. |
| Crunchbase | `https://mcp.crunchbase.com/` | `sfx-sales` | Your own Crunchbase account | Sign-in required (401) | None. |
| Databricks | (blank) | `sfx-finance`, `sfx-data` | Your own Databricks account and its MCP address | Placeholder | Blank on purpose. Every account has its own MCP address. Ask your data admin for it, then add the server in your app. |
| Datadog | `https://mcp.datadoghq.com/api/unstable/mcp-server/mcp` | `sfx-engineering` | Your own Datadog account | Account required (401) | This address is for accounts on datadoghq.com. An account on another Datadog site needs that site's MCP address. |
| Definite | (blank) | `sfx-data` | Your own Definite deployment address | Placeholder | Blank on purpose. The upstream address `https://api.definite.app/v3/mcp/http` returned HTTP 404 on September 27, 2026, and Definite now documents MCP at your own deployment address. |
| Docusign | `https://mcp.docusign.com/mcp` | `sfx-small-business`, `sfx-legal` | Your own Docusign account | Refused anonymous check (403) | The server refused an anonymous check on September 27, 2026, so it could not be verified without an account. Its tools may include sending documents for signature. Read every action before you approve it. |
| Egnyte | `https://mcp-server.egnyte.com/mcp` | `sfx-legal` | Your own Egnyte account | Sign-in required (401) | None. |
| Emergent | `https://mcp.emergent.sh` | `sfx-small-business` | Your own Emergent account | Sign-in required (401) | None. |
| Expensify | `https://www.expensify.com/mcp` | `sfx-small-business` | Your own Expensify account | Reachable, redirects (308) | Its tools may include expense reports and approvals. Read every action before you approve it. |
| Figma | `https://mcp.figma.com/mcp` | `sfx-marketing`, `sfx-design`, `sfx-product-management` | Your own Figma account | Sign-in required (401) | None. |
| Fireflies | `https://api.fireflies.ai/mcp` | `sfx-sales`, `sfx-product-management` | Your own Fireflies account | Sign-in required (401) | None. |
| GitHub | `https://api.githubcopilot.com/mcp/` | `sfx-engineering` | Your own GitHub account | Sign-in required (401) | None. |
| Gmail | (blank) | `sfx-marketing`, `sfx-sales`, `sfx-customer-support`, `sfx-operations`, `sfx-finance`, `sfx-human-resources`, `sfx-productivity`, `sfx-legal`, `sfx-design`, `sfx-enterprise-search`, `sfx-product-management`, `sfx-engineering` | Your own Gmail account | Placeholder | Blank on purpose, so it shows as "not configured" instead of an error. Connect Gmail from your Claude connector settings, or add Google's MCP server yourself. The skills use any email tool you connect. |
| Gmail | `https://gmailmcp.googleapis.com/mcp/v1` | `sfx-small-business` | Your own Gmail account | Reachable (200) | Signs in with Google. If Claude Code reports that the server does not support dynamic client registration, create an OAuth client in your own Google Cloud project and add the server with `--client-id`. |
| Gong | `https://mcp.gong.io/mcp` | `sfx-sales` | Your own Gong account | Sign-in required (401) | None. |
| Google Calendar | (blank) | `sfx-marketing`, `sfx-sales`, `sfx-customer-support`, `sfx-operations`, `sfx-finance`, `sfx-human-resources`, `sfx-productivity`, `sfx-legal`, `sfx-design`, `sfx-enterprise-search`, `sfx-product-management`, `sfx-engineering` | Your own Google Calendar account | Placeholder | Blank on purpose, so it shows as "not configured" instead of an error. Connect Google Calendar from your Claude connector settings, or add Google's MCP server yourself. The skills use any calendar tool you connect. |
| Google Calendar | `https://calendarmcp.googleapis.com/mcp/v1` | `sfx-small-business` | Your own Google Calendar account | Reachable (200) | Signs in with Google. If Claude Code reports that the server does not support dynamic client registration, create an OAuth client in your own Google Cloud project and add the server with `--client-id`. |
| Google Drive | (blank) | `sfx-sales` | Your own Google Drive account | Placeholder | Blank on purpose, so it shows as "not configured" instead of an error. Connect Google Drive from your Claude connector settings, or add Google's MCP server yourself. The skills use any file storage tool you connect. |
| Google Drive | `https://drivemcp.googleapis.com/mcp/v1` | `sfx-small-business` | Your own Google Drive account | Reachable (200) | Signs in with Google. If Claude Code reports that the server does not support dynamic client registration, create an OAuth client in your own Google Cloud project and add the server with `--client-id`. |
| Guru | `https://mcp.api.getguru.com/mcp` | `sfx-customer-support`, `sfx-enterprise-search` | Your own Guru account | Sign-in required (401) | None. |
| Gusto | `https://mcp.api.gusto.com/anthropic` | `sfx-small-business` | Your own Gusto account | Sign-in required (401) | The vendor runs this address for Claude apps. Its tools may include payroll changes. Read every action before you approve it. |
| Hex | `https://app.hex.tech/mcp` | `sfx-data` | Your own Hex account | Sign-in required (401) | None. |
| HubSpot | `https://mcp.hubspot.com/anthropic` | `sfx-small-business`, `sfx-marketing`, `sfx-sales`, `sfx-customer-support` | Your own HubSpot account | Sign-in required (401) | The vendor runs this address for Claude apps. |
| Intercom | `https://mcp.intercom.com/mcp` | `sfx-customer-support`, `sfx-design`, `sfx-product-management` | Your own Intercom account | Sign-in required (401) | None. |
| Klaviyo | `https://mcp.klaviyo.com/mcp` | `sfx-marketing` | Your own Klaviyo account | Sign-in required (401) | None. |
| Linear | `https://mcp.linear.app/mcp` | `sfx-productivity`, `sfx-design`, `sfx-product-management`, `sfx-engineering` | Your own Linear account | Sign-in required (401) | None. |
| Lusha | `https://mcp.lusha.com/mcp/claude` | `sfx-sales` | Your own Lusha account | Sign-in required (401) | The vendor runs this address for Claude apps. |
| Mailchimp | `https://ai-inc.mailchimp.com/claude/mcp/v2` | `sfx-small-business` | Your own Mailchimp account | Refused anonymous check (403) | The vendor runs this address for Claude apps. The server refused an anonymous check on September 27, 2026, so it could not be verified without an account. |
| Microsoft 365 | `https://microsoft365.mcp.claude.com/mcp` | `sfx-sales` | Your own Microsoft 365 work account, with admin setup | Sign-in required (401) | An admin enables this connector in Claude before people can sign in. The address is hosted by Anthropic for Claude apps and was not verified outside them. |
| monday.com | `https://mcp.monday.com/mcp` | `sfx-small-business`, `sfx-sales`, `sfx-productivity`, `sfx-product-management` | Your own monday.com account | Sign-in required (401) | None. |
| MYOB | `https://mcp.myob.com/mcp` | `sfx-small-business` | Your own MYOB account | Sign-in required (401) | Its tools may include creating and changing accounting records. Read every action before you approve it. |
| Notion | `https://mcp.notion.com/mcp` | `sfx-small-business`, `sfx-marketing`, `sfx-sales`, `sfx-customer-support`, `sfx-operations`, `sfx-human-resources`, `sfx-productivity`, `sfx-design`, `sfx-enterprise-search`, `sfx-product-management`, `sfx-engineering` | Your own Notion account | Sign-in required (401) | None. |
| Otter.ai | `https://mcp.otter.ai/mcp` | `sfx-sales` | Your own Otter.ai account | Sign-in required (401) | None. |
| Outreach | `https://api.outreach.io/mcp/` | `sfx-sales` | Your own Outreach account | Sign-in required (401) | None. |
| PagerDuty | `https://mcp.pagerduty.com/mcp` | `sfx-engineering` | Your own PagerDuty account | Sign-in required (401) | None. |
| PayPal | `https://mcp.paypal.com/mcp` | `sfx-small-business` | Your own PayPal account | Sign-in required (401) | Its tools may include payments, refunds and invoices. Read every action before you approve it. |
| PDF server (local) | `npx -y @modelcontextprotocol/server-pdf@2.0.3 --stdio` | `sfx-pdf-viewer` | Node.js 20 or later on your computer | Local | Runs on your computer with `npx`. The first run downloads `@modelcontextprotocol/server-pdf` version 2.0.3 from npm. The version is pinned, so a new npm release does not change what runs. Version 2.0.3 requires Node.js 20 or later. No account or API key. |
| Pendo | `https://app.pendo.io/mcp/v0/shttp` | `sfx-product-management` | Your own Pendo account | Sign-in required (401) | None. |
| QuickBooks | `https://ai-inc.quickbooks.intuit.com/v1/mcp` | `sfx-small-business` | Your own QuickBooks account | Refused anonymous check (403) | The server refused an anonymous check on September 27, 2026, so it could not be verified without an account. Its tools may include creating and changing accounting records. Read every action before you approve it. |
| Ramp | `https://mcp.ramp.com/mcp` | `sfx-small-business` | Your own Ramp account | Sign-in required (401) | Its tools may include cards, bills and payments. Read every action before you approve it. |
| RingCentral team chat | `https://mcp.labs.ringcentral.com/ringex/v1.1.0/team-chat` | `sfx-small-business` | Your own RingCentral team chat account | Sign-in required (401) | None. |
| Salesforce | `https://api.salesforce.com/platform/mcp/v1/platform/headless-360` | `sfx-sales` | Your own Salesforce org, with admin setup | Account required (401) | An admin enables this connector in Claude and sets up your org's Salesforce app before people can sign in. |
| Shopify | `https://setup.shopify.com/mcp` | `sfx-small-business` | Your own Shopify account | Reachable (200) | Answers without sign-in for store setup and sample catalogs. Your own store data needs your Shopify sign-in. Its tools may include changes to products, prices, inventory and orders. Read every action before you approve it. |
| Similarweb | `https://mcp.similarweb.com` | `sfx-marketing` | Your own Similarweb account | Sign-in required (401) | None. |
| Similarweb | `https://mcp.similarweb.com/mcp` | `sfx-sales`, `sfx-product-management` | Your own Similarweb account | Sign-in required (401) | None. |
| Slack | `https://mcp.slack.com/mcp` | `sfx-small-business`, `sfx-marketing`, `sfx-sales`, `sfx-customer-support`, `sfx-operations`, `sfx-finance`, `sfx-human-resources`, `sfx-productivity`, `sfx-legal`, `sfx-design`, `sfx-enterprise-search`, `sfx-product-management`, `sfx-engineering` | Your own Slack workspace, with admin approval | Sign-in required (401) | Uses the sign-in app Slack publishes for Claude Code. A workspace admin must approve the Slack MCP app. |
| Snowflake | (blank) | `sfx-finance`, `sfx-data` | Your own Snowflake account and its MCP address | Placeholder | Blank on purpose. Every account has its own MCP address. Ask your data admin for it, then add the server in your app. |
| Square | `https://mcp.squareup.com/mcp` | `sfx-small-business` | Your own Square account | Sign-in required (401) | Its tools may include payments, refunds and invoices. Read every action before you approve it. |
| Stripe | `https://mcp.stripe.com` | `sfx-small-business` | Your own Stripe account | Sign-in required (401) | Its tools may include payments, refunds and invoices. Read every action before you approve it. |
| Supermetrics | `https://mcp.supermetrics.com/mcp` | `sfx-marketing` | Your own Supermetrics account | Sign-in required (401) | None. |
| TikTok Ads | `https://business-api.tiktok.com/open_mcp/tt-ads-mcp-layer` | `sfx-small-business` | Your own TikTok Ads account | Sign-in required (401) | None. |
| Trello | `https://mcp.trello.com/v1` | `sfx-small-business` | Your own Trello account | Sign-in required (401) | None. |
| Wix | `https://mcp.wix.com/mcp` | `sfx-small-business` | Your own Wix account | Sign-in required (401) | None. |
| Xero | `https://mcp.xero.com/mcp` | `sfx-small-business` | Your own Xero account | Sign-in required (401) | Its tools may include creating and changing accounting records. Read every action before you approve it. |
| Zapier | `https://mcp.zapier.com/api/v1/connect` | `sfx-small-business` | Your own Zapier account | Sign-in required (401) | None. |
| Zoho Books | `https://claude-zohobooks.zohomcp.com/mcp/message` | `sfx-small-business` | Your own Zoho Books account | Sign-in required (401) | The vendor runs this address for Claude apps. Its tools may include creating and changing accounting records. Read every action before you approve it. |
| Zoho CRM | `https://claude-zohocrm.zohomcp.com/mcp/message` | `sfx-small-business` | Your own Zoho CRM account | Sign-in required (401) | The vendor runs this address for Claude apps. |
| Zoho Desk | `https://claude-zohodesk.zohomcp.com/mcp/message` | `sfx-small-business` | Your own Zoho Desk account | Sign-in required (401) | The vendor runs this address for Claude apps. |
| Zoho Projects | `https://claude-zohoprojects.zohomcp.com/mcp/message` | `sfx-small-business` | Your own Zoho Projects account | Sign-in required (401) | The vendor runs this address for Claude apps. |
| Zoom | `https://mcp.zoom.us/mcp/zoom/streamable` | `sfx-small-business`, `sfx-sales` | Your own Zoom account | Sign-in required (401) | None. |
| ZoomInfo | `https://mcp.zoominfo.com/mcp` | `sfx-sales` | Your own ZoomInfo account | Sign-in required (401) | None. |

## What SMILE-FX changed

- Definite: the upstream address `https://api.definite.app/v3/mcp/http` returned HTTP 404 on September 27, 2026, so the entry in `sfx-data` is now a blank placeholder.
- PDF server: `sfx-pdf-viewer` runs `@modelcontextprotocol/server-pdf@2.0.3` instead of the newest version on npm, so a new npm release does not change what runs until SMILE-FX releases a new plugin version.
- Every other address is the one upstream shipped. The Slack entry keeps the client ID that Slack publishes for Claude Code.

Company names are trademarks of their owners and are named only to describe compatibility.

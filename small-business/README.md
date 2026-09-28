# SMILE-FX® Small Business

> Runs the business side of a practice or small business: cash, bills, payroll prep, sales follow-up, marketing, reviews and hiring. Ask in plain words and it picks the right workflow. It asks before anything sends, posts or pays.

**Install id:** `sfx-small-business` | **Version:** 1.0.0 | **Skills:** 44 | **Commands:** 0 | **Licence:** Apache-2.0

## Who it is for

Owners and office managers who run the business side of a practice: cash, bills, payroll prep, marketing, reviews and hiring.

## Install

**Claude Code.** In a session:

```text
/plugin marketplace add wherewolf87/smile-fx-plugins
/plugin install sfx-small-business@smile-fx-plugins
```

The install command opens the plugin panel so you can review it and pick a scope. From your shell, use `claude plugin marketplace add wherewolf87/smile-fx-plugins` and `claude plugin install sfx-small-business@smile-fx-plugins`.

**Cowork.** Open **Customize**, then **Plugins**. Select **Add**, then **Add marketplace**, and enter `wherewolf87/smile-fx-plugins`. Select **SMILE-FX Small Business** and **Install**, then connect your tools on its **Connectors** tab. Plugins need a paid Claude plan.

Full steps: [install guide](../README.md#install).

## Try asking

- "Get me started."
- "Which bills are due in the next 14 days, and can we cover them?"
- "Draft a job post and interview guide for a front desk coordinator."

## First run

Start with "Get me started." The `smb-onboard` skill connects your first two tools, runs one workflow and saves a short profile of your business so later skills need less explaining. It shows you the profile and asks before it saves.

## Skills (44)

Claude uses a skill when your request matches it. You can also call one by name.

| Skill | What it does |
|---|---|
| `/sfx-small-business:ad-manager` | Reads ad results, explains what works and what wastes money, and drafts budget and creative changes for approval. |
| `/sfx-small-business:ap-processor` | Reads and codes incoming bills, matches them to orders, and stages entries and a payment run for your approval. |
| `/sfx-small-business:brand-style` | Captures your brand look and output preferences so every report and document follows them. |
| `/sfx-small-business:build-agent` | Turns a task you repeat by hand into a named skill you can run on demand or on a schedule. |
| `/sfx-small-business:build-connector` | Connects a tool that has no ready-made connector, through Zapier, with approval gates on anything that writes. |
| `/sfx-small-business:business-pulse` | One-page snapshot of cash, sales, pipeline, this week's commitments and the item that needs you today. |
| `/sfx-small-business:call-list` | Builds today's call list with talking points, calendar blocks and drafted follow-ups. |
| `/sfx-small-business:canva-creator` | Turns an approved content brief into a posting calendar, Canva designs and drafted captions and emails. |
| `/sfx-small-business:cash-flow-snapshot` | Forecasts cash 30, 60 and 90 days out from your ledger, payment tools or a CSV, with named risk flags. |
| `/sfx-small-business:close-month` | Runs month-end in order: reconcile, refresh the cash forecast, then publish the close packet. |
| `/sfx-small-business:content-strategy` | Finds what sells and what stalls, adds seasonality, and writes a 30-day content brief. |
| `/sfx-small-business:contract-review` | Flags non-standard terms in NDAs, service agreements and vendor contracts, with a redline for your counsel. |
| `/sfx-small-business:crm-autopilot` | Keeps contacts, deals and activity in your CRM current from email, calendar and call notes. |
| `/sfx-small-business:grant-rfp-writer` | Finds grants and solicitations you qualify for, runs a go or no-go check, drafts the response and tracks deadlines. |
| `/sfx-small-business:grow-pipeline` | Researches the market, builds a ranked prospect list, drafts outreach in your voice and logs it to the CRM. |
| `/sfx-small-business:growth-pulse` | Checks whether growth is working: sales by channel, funnel, campaign return and customer sentiment. |
| `/sfx-small-business:hiring-screener` | Scores applications against your stated rubric, drafts replies, schedules interviews and preps onboarding. |
| `/sfx-small-business:inbox-manager` | Sorts a full inbox into what needs you, drafts replies and pulls out action items and deadlines. |
| `/sfx-small-business:inventory-planner` | Works out what to reorder and when from sales and stock on hand, and drafts purchase orders. |
| `/sfx-small-business:invoice-chase` | Drafts overdue invoice reminders matched to each customer's payment history. |
| `/sfx-small-business:job-post-builder` | Builds a hiring packet from a brief: job post, interview guide with scoring rubric and offer letter template. |
| `/sfx-small-business:lead-finder` | Builds a ranked list of prospects that look like your current customers, with contacts and signals. |
| `/sfx-small-business:lead-triage` | Scores inbound HubSpot leads, ranks the ones worth a call today and drafts follow-ups. |
| `/sfx-small-business:marketing-monday` | Weekly growth briefing: what works, what customers say, what competitors changed and three actions. |
| `/sfx-small-business:monday-brief` | Monday morning briefing on one page: business snapshot, saved KPI reports and the week ahead. |
| `/sfx-small-business:month-end-prep` | Reconciles the ledger against payment settlements, flags issues and writes a plain-language P&L narrative. |
| `/sfx-small-business:outreach-composer` | Writes prospect outreach and follow-up sequences in your own voice and queues each send for approval. |
| `/sfx-small-business:pay-the-bills` | Takes bills from the inbox to a staged payment run after a cash check, ready for one approval. |
| `/sfx-small-business:payroll-prep` | Totals hours from timesheets, flags anomalies and stages payroll for line-by-line approval. |
| `/sfx-small-business:plan-payroll` | Payroll readiness in one pass: cash forecast, overdue invoice reminders, then payroll prep. |
| `/sfx-small-business:proposal-builder` | Turns call notes, photos or an RFP into a costed proposal or statement of work on your templates. |
| `/sfx-small-business:reactivate` | Finds customers who stopped buying, ranks them and drafts win-back messages for approval. |
| `/sfx-small-business:report-builder` | Turns a plain-words description of a recurring report into a repeatable report with a workbook. |
| `/sfx-small-business:report-pack` | Runs your saved reports on a set cadence with a business snapshot for context. |
| `/sfx-small-business:restock` | Turns sales velocity into a reorder, a purchase order, a vendor email and a matching ledger entry. |
| `/sfx-small-business:review-reputation` | Groups public reviews and private feedback into themes, drafts review replies and spots customers at risk. |
| `/sfx-small-business:seo-ai-visibility` | Audits how people and AI assistants find your site, and drafts the fixes. |
| `/sfx-small-business:smb-onboard` | Guided setup: connects your first two tools, runs one workflow and learns your business. |
| `/sfx-small-business:smb-router` | The front door: explains what the plugin can do and routes your request to the right skill. |
| `/sfx-small-business:social-content-engine` | Keeps a rolling posting calendar, drafts on-brand graphics and captions, and stages posts for approval. |
| `/sfx-small-business:speed-to-lead` | Drafts a reply to every new inquiry with real meeting times, for you to approve and send. |
| `/sfx-small-business:tax-prep` | Confirms the books are closed, then prepares quarterly estimates or the year-end 1099 list for your accountant. |
| `/sfx-small-business:tax-season-organizer` | Prepares tax-season material for your accountant. Not tax advice. |
| `/sfx-small-business:ticket-deflector` | Reads a customer email or ticket, checks orders and history, and drafts a reply. Refunds only with your approval. |

## Connectors

Set up: Airwallex, Apollo, Atlassian (Jira, Confluence), Canva, Clay, Docusign, Emergent, Expensify, Gmail, Google Calendar, Google Drive, Gusto, HubSpot, Mailchimp, QuickBooks, monday.com, MYOB, Notion, PayPal, Ramp, RingCentral team chat, Shopify, Slack, Square, Stripe, TikTok Ads, Trello, Wix, Xero, Zapier, Zoho Books, Zoho CRM, Zoho Desk, Zoho Projects, Zoom.

Each connector signs in with your own account, and nothing connects until you do. [CONNECTORS.md](CONNECTORS.md) lists what each one needs.

These connectors can take actions such as payments, payroll, record changes or e-signature requests: Airwallex, Docusign, Expensify, Gusto, QuickBooks, MYOB, PayPal, Ramp, Shopify, Square, Stripe, Xero, Zoho Books. Read every action before you approve it.

## Good to know

- The skills are written to pause for your approval before anything sends, posts, pays or changes a record.
- Tax and payroll skills prepare material for your accountant or payroll provider. They are not tax or legal advice.
- Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.
- Software suggests. People decide. Check what a skill produces before you use it.

## Credits and licence

Adapted by SMILE-FX P.A. from the `small-business` plugin in Anthropic's [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) (commit `da38ec1`), under the Apache License 2.0. SMILE-FX changed the plugin name and metadata, this README, the connector notes, skill text that named the old plugin, one line of reference text about the plugin's positioning, and punctuation in skill descriptions (long dashes replaced with commas or colons). The changes are listed in [MODIFICATIONS.md](../MODIFICATIONS.md). Licence: [LICENSE](LICENSE). Notices: [NOTICE](../NOTICE).

© 2026 SMILE-FX P.A. SMILE-FX® is a registered trademark of SMILE-FX P.A. SMILE-FX P.A. is not affiliated with, sponsored by or endorsed by Anthropic. Anthropic, Claude, Claude Code and Claude Cowork are trademarks of Anthropic, PBC. They are named here only to describe compatibility.

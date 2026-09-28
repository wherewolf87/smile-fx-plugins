<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/smile-fx-logo-on-dark.svg">
    <img alt="SMILE-FX" src="assets/smile-fx-logo-on-light.svg" width="420">
  </picture>
</p>

<h1 align="center">SMILE-FX® Plugins</h1>

<p align="center"><strong>16 free plugins that teach Claude the business side of a practice.</strong><br>
Marketing, sales, front desk, finance, HR, operations, legal and more. Install one in a minute.</p>

<p align="center">
  <img alt="Licence: Apache-2.0" src="https://img.shields.io/badge/licence-Apache--2.0-08E8F6?labelColor=000000">
  <img alt="16 plugins" src="https://img.shields.io/badge/plugins-16-08E8F6?labelColor=000000">
  <img alt="175 skills" src="https://img.shields.io/badge/skills-175-08E8F6?labelColor=000000">
</p>

<p align="center">
  <a href="#install">Install</a> ·
  <a href="#the-plugins">The plugins</a> ·
  <a href="#connectors">Connectors</a> ·
  <a href="#patient-health-information">Health data</a> ·
  <a href="#credits-and-licence">Credits</a>
</p>

## What this is

A plugin is a folder of written know-how that Claude loads when you need it. Each SMILE-FX plugin covers one part of running a business. It adds **skills**, step-by-step instructions for a job such as "prep my call" or "reconcile this bank export", and **connectors**, sign-in links to the tools you already use, such as your CRM, email or accounting software.

You ask in plain words. Claude picks the matching skill, asks for what it needs and does the work. Your app's permission settings decide whether a connected tool runs straight away or asks you first, so keep anything that sends, posts, pays or changes a record on ask. You can also call a skill by name, for example `/sfx-marketing:draft-content`.

All 16 plugins install in Claude Code and in Cowork in the Claude desktop app. SMILE-FX Plugin Builder is written for Cowork first.

## Who it is for

Practice and business owners, office managers and the small teams around them: dental and orthodontic practices, clinics, studios, agencies and local service businesses. You do not need to write code. If you can describe the job, the plugin can help with it.

## The plugins

16 plugins, 175 skills and 5 commands. Counts come from the files in this repository. Claude Code shows commands in the same list as skills.

| Plugin | Install id | What it does | Skills | Commands |
|---|---|---|---:|---:|
| [SMILE-FX Small Business](small-business/README.md) | `sfx-small-business` | Runs the business side of a practice or small business: cash, bills, payroll prep, sales follow-up, marketing, reviews and hiring. | 44 | 0 |
| [SMILE-FX Marketing](marketing/README.md) | `sfx-marketing` | Plans campaigns, drafts content, checks brand voice, audits SEO and reports on results across your marketing channels. | 8 | 0 |
| [SMILE-FX Sales](sales/README.md) | `sfx-sales` | Preps calls, summarizes meetings, drafts follow-ups, researches accounts and reviews your pipeline, using your CRM, email, calendar and call notes, or uploaded files. | 36 | 0 |
| [SMILE-FX Customer Support](customer-support/README.md) | `sfx-customer-support` | Triages questions, drafts replies, packages escalations and turns resolved questions into help articles. | 5 | 0 |
| [SMILE-FX Operations](operations/README.md) | `sfx-operations` | Documents processes, reviews vendors, plans capacity, tracks compliance tasks and writes status reports. | 9 | 0 |
| [SMILE-FX Finance](finance/README.md) | `sfx-finance` | Prepares journal entries, reconciliations, financial statements and variance analysis, and supports month-end close and audit prep. | 8 | 0 |
| [SMILE-FX Human Resources](human-resources/README.md) | `sfx-human-resources` | Supports recruiting, onboarding, performance reviews, compensation analysis and policy questions. | 9 | 0 |
| [SMILE-FX Productivity](productivity/README.md) | `sfx-productivity` | Keeps a task list and a working memory of your people, projects and shorthand, and pulls new tasks from your calendar, email and chat. | 4 | 0 |
| [SMILE-FX Legal](legal/README.md) | `sfx-legal` | Reviews contracts against your playbook, triages NDAs, checks compliance questions and drafts briefings for your counsel. | 9 | 0 |
| [SMILE-FX Data](data/README.md) | `sfx-data` | Writes SQL, explores data sets, runs statistics, builds charts and dashboards, and checks an analysis before you share it. | 10 | 0 |
| [SMILE-FX Design](design/README.md) | `sfx-design` | Critiques designs, writes interface copy, reviews accessibility, synthesizes research and prepares developer handoff notes. | 7 | 0 |
| [SMILE-FX Enterprise Search](enterprise-search/README.md) | `sfx-enterprise-search` | Searches your email, chat, documents and wikis in one request, and writes digests of what changed. | 5 | 0 |
| [SMILE-FX Product Management](product-management/README.md) | `sfx-product-management` | Writes specs, plans roadmaps and sprints, synthesizes research, reviews metrics and drafts stakeholder updates. | 8 | 1 |
| [SMILE-FX PDF Viewer](pdf-viewer/README.md) | `sfx-pdf-viewer` | Opens PDFs in an interactive viewer so you can read, annotate, fill forms and place signatures, then download the marked-up copy. | 1 | 4 |
| [SMILE-FX Engineering](engineering/README.md) | `sfx-engineering` | Supports standups, code review, debugging, architecture decisions, incident response and technical documentation. | 10 | 0 |
| [SMILE-FX Plugin Builder](plugin-builder/README.md) | `sfx-plugin-builder` | Builds new plugins from scratch and customizes existing ones for your own tools, terms and workflows. | 2 | 0 |
| **Total** | | | **175** | **5** |

<details>
<summary><strong>Every skill, by plugin</strong></summary>

**SMILE-FX Small Business** (`sfx-small-business`): `ad-manager`, `ap-processor`, `brand-style`, `build-agent`, `build-connector`, `business-pulse`, `call-list`, `canva-creator`, `cash-flow-snapshot`, `close-month`, `content-strategy`, `contract-review`, `crm-autopilot`, `grant-rfp-writer`, `grow-pipeline`, `growth-pulse`, `hiring-screener`, `inbox-manager`, `inventory-planner`, `invoice-chase`, `job-post-builder`, `lead-finder`, `lead-triage`, `marketing-monday`, `monday-brief`, `month-end-prep`, `outreach-composer`, `pay-the-bills`, `payroll-prep`, `plan-payroll`, `proposal-builder`, `reactivate`, `report-builder`, `report-pack`, `restock`, `review-reputation`, `seo-ai-visibility`, `smb-onboard`, `smb-router`, `social-content-engine`, `speed-to-lead`, `tax-prep`, `tax-season-organizer`, `ticket-deflector`

**SMILE-FX Marketing** (`sfx-marketing`): `brand-review`, `campaign-plan`, `competitive-brief`, `content-creation` (automatic), `draft-content`, `email-sequence`, `performance-report`, `seo-audit`

**SMILE-FX Sales** (`sfx-sales`): `account-context`, `account-plan`, `account-research`, `account-tiering`, `call-prep`, `call-summary`, `close-plan`, `competitive-intelligence`, `create-an-asset`, `crm-hygiene-check`, `customer-health`, `customer-voice`, `daily-briefing`, `deal-advance-gap`, `deal-review`, `deal-signals`, `deal-slip-scenario`, `draft-outreach`, `end-of-day`, `expansion-whitespace`, `forecast`, `handle-objection`, `inbox-sweep`, `lead-triage`, `log-activity`, `pipeline-review`, `renewal-radar`, `rep-context`, `route-lead`, `schedule-meeting`, `setup`, `stakeholder-map`, `team-pipeline`, `update-opportunity`, `weekly-wrap`, `win-loss-review`

**SMILE-FX Customer Support** (`sfx-customer-support`): `customer-escalation`, `customer-research`, `draft-response`, `kb-article`, `ticket-triage`

**SMILE-FX Operations** (`sfx-operations`): `capacity-plan`, `change-request`, `compliance-tracking`, `process-doc`, `process-optimization`, `risk-assessment`, `runbook`, `status-report`, `vendor-review`

**SMILE-FX Finance** (`sfx-finance`): `audit-support` (automatic), `close-management` (automatic), `financial-statements`, `journal-entry`, `journal-entry-prep` (automatic), `reconciliation`, `sox-testing`, `variance-analysis`

**SMILE-FX Human Resources** (`sfx-human-resources`): `comp-analysis`, `draft-offer`, `interview-prep`, `onboarding`, `org-planning`, `people-report`, `performance-review`, `policy-lookup`, `recruiting-pipeline`

**SMILE-FX Productivity** (`sfx-productivity`): `memory-management` (automatic), `start`, `task-management` (automatic), `update`

**SMILE-FX Legal** (`sfx-legal`): `brief`, `compliance-check`, `legal-response`, `legal-risk-assessment`, `meeting-briefing`, `review-contract`, `signature-request`, `triage-nda`, `vendor-check`

**SMILE-FX Data** (`sfx-data`): `analyze`, `build-dashboard`, `create-viz`, `data-context-extractor`, `data-visualization` (automatic), `explore-data`, `sql-queries` (automatic), `statistical-analysis` (automatic), `validate-data`, `write-query`

**SMILE-FX Design** (`sfx-design`): `accessibility-review`, `design-critique`, `design-handoff`, `design-system`, `research-synthesis`, `user-research`, `ux-copy`

**SMILE-FX Enterprise Search** (`sfx-enterprise-search`): `digest`, `knowledge-synthesis` (automatic), `search`, `search-strategy` (automatic), `source-management` (automatic)

**SMILE-FX Product Management** (`sfx-product-management`): `competitive-brief`, `metrics-review`, `product-brainstorming`, `roadmap-update`, `sprint-planning`, `stakeholder-update`, `synthesize-research`, `write-spec`; commands: `brainstorm`

**SMILE-FX PDF Viewer** (`sfx-pdf-viewer`): `view-pdf`; commands: `annotate`, `fill-form`, `open`, `sign`

**SMILE-FX Engineering** (`sfx-engineering`): `architecture`, `code-review`, `debug`, `deploy-checklist`, `documentation`, `incident-response`, `standup`, `system-design`, `tech-debt`, `testing-strategy`

**SMILE-FX Plugin Builder** (`sfx-plugin-builder`): `create-plugin`, `customize-plugin`

Skills marked automatic have no slash command. Claude uses them when your request needs them.

</details>

## Install

### Claude Code

In a Claude Code session (terminal, desktop app Code tab or VS Code), add the marketplace once, then install the plugins you want:

```text
/plugin marketplace add wherewolf87/smile-fx-plugins
/plugin install sfx-marketing@smile-fx-plugins
```

The install command opens the plugin panel so you can review what it adds and choose a scope. Replace `sfx-marketing` with any install id from the table.

From your shell:

```bash
claude plugin marketplace add wherewolf87/smile-fx-plugins
claude plugin install sfx-marketing@smile-fx-plugins
```

One step, on Claude Code 2.1.275 or later: `/plugin install sfx-marketing --marketplace wherewolf87/smile-fx-plugins`.

Skills then run as `/<install id>:<skill>`, for example `/sfx-marketing:draft-content`. Skills marked automatic in the plugin lists have no slash command.

To share plugins with everyone who works in a repository, run `claude plugin marketplace add wherewolf87/smile-fx-plugins --scope project` from your shell in that repository and commit `.claude/settings.json`. Each person then runs `claude plugin install <install id>@smile-fx-plugins --scope project` once.

### Cowork (Claude desktop app)

1. Open **Cowork**, then **Customize** in the left sidebar, then **Plugins**.
2. Select **Add**, then **Add marketplace**, and enter `wherewolf87/smile-fx-plugins` (or `https://github.com/wherewolf87/smile-fx-plugins`).
3. Select a SMILE-FX plugin, then **Install**.
4. Open the plugin's **Connectors** tab and connect the tools you use. Installing does not sign you in to anything.

Plugins need a paid Claude plan: Pro, Max, Team or Enterprise. Plugins you add in Cowork are saved to your Claude account.

Cowork adds Anthropic's Knowledge Work marketplace by default. Its plugins and these SMILE-FX plugins cover many of the same roles, so install one version of each role to avoid duplicate skills.

### Updates

Automatic updates for third-party marketplaces are off by default. To turn them on in Claude Code, run `/plugin`, open **Marketplaces**, select `smile-fx-plugins` and choose **Enable auto-update**. To update by hand, run `/plugin marketplace update smile-fx-plugins` to refresh the list, then open each plugin on the **Installed** tab in `/plugin` and select **Update now**. From your shell: `claude plugin marketplace update smile-fx-plugins`, then `claude plugin update sfx-marketing@smile-fx-plugins`. An update loads in your next session, or when you run `/reload-plugins`.

In Cowork, select **Check for updates** on the marketplace, or turn on **Sync automatically**.

## Your first ten minutes

1. Install **SMILE-FX Small Business** and say "Get me started." It connects your first two tools and learns the basics of your business.
2. Ask for one real job you do every week, such as "Which bills are due in the next 14 days?" or "Draft replies to the questions in my inbox."
3. Read the result. Change what is wrong and tell Claude why, so the next answer fits your practice.
4. Add the department plugins you need, such as Marketing, Sales or Human Resources.

## Connectors

Most plugins come with connectors already listed, such as Slack, HubSpot, Notion, QuickBooks or Stripe. Each one signs in with **your own account** for that service. A few entries are blank on purpose (Gmail, Google Calendar, Google Drive, Snowflake, Databricks and Definite in some plugins) because each account has its own address or sign-in. Claude Code shows those as "not configured" instead of an error.

Some connectors can take actions such as payments, payroll or record changes. Your app's permission settings decide whether each tool runs straight away or asks you first. Keep those on ask. [CONNECTORS.md](CONNECTORS.md) lists every connector, what it needs and what we saw when we checked it.

## Patient health information

Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test. These plugins do not give clinical, legal, tax or financial advice. Software suggests. People decide.

## Make them yours

- **SMILE-FX Plugin Builder** (`sfx-plugin-builder`) creates new plugins and adapts these ones to your tools and terms.
- Each plugin's CONNECTORS.md explains the `~~category` placeholders, so you can swap in the tools you use.
- Everything here is plain text you can read before you install it.

## Security

Only install plugins you trust, and review what a plugin adds before you install it. Report security problems privately as described in [SECURITY.md](SECURITY.md).

## More from SMILE-FX

This repository is one of three free resources from SMILE-FX®. The AI Operating System playbook and the department prompt library are at [smile-fx-ai.vercel.app](https://smile-fx-ai.vercel.app). Plugin page: [smile-fx-ai.vercel.app/plugins](https://smile-fx-ai.vercel.app/plugins).

## Credits and licence

SMILE-FX® Plugins adapts 16 plugins from Anthropic's open-source [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) at commit `da38ec1` (September 24, 2026), under the Apache License 2.0. SMILE-FX P.A. renamed and rebranded them, rewrote the documentation and adjusted connector setup. Skill instructions are unchanged apart from renamed references and the punctuation of some skill descriptions (long dashes replaced with commas or colons).

- Licence: [LICENSE](LICENSE) (Apache License 2.0, also in every plugin folder)
- Attribution: [NOTICE](NOTICE)
- Every change: [MODIFICATIONS.md](MODIFICATIONS.md)
- Release history: [CHANGELOG.md](CHANGELOG.md)
- How to help: [CONTRIBUTING.md](CONTRIBUTING.md)

© 2026 SMILE-FX P.A. SMILE-FX® is a registered trademark of SMILE-FX P.A. The logo files in `assets/` are not licensed under the Apache License.

SMILE-FX P.A. is not affiliated with, sponsored by or endorsed by Anthropic. Anthropic, Claude, Claude Code and Claude Cowork are trademarks of Anthropic, PBC. They are named here only to describe compatibility. Other product names are trademarks of their owners. Naming a product does not mean its maker endorses or sponsors SMILE-FX®.

<p align="center"><em>Elevating Smiles, Elevating You</em></p>

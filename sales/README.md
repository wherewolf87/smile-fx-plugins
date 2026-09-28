# SMILE-FX® Sales

> Preps calls, summarizes meetings, drafts follow-ups, researches accounts and reviews your pipeline, using your CRM, email, calendar and call notes, or uploaded files. It updates records or sends email only when you ask.

**Install id:** `sfx-sales` | **Version:** 1.0.0 | **Skills:** 36 | **Commands:** 0 | **Licence:** Apache-2.0

## Who it is for

Practices that track relationships in a CRM: referral partners, employers, vendors and group agreements.

## Install

**Claude Code.** In a session:

```text
/plugin marketplace add wherewolf87/smile-fx-plugins
/plugin install sfx-sales@smile-fx-plugins
```

The install command opens the plugin panel so you can review it and pick a scope. From your shell, use `claude plugin marketplace add wherewolf87/smile-fx-plugins` and `claude plugin install sfx-sales@smile-fx-plugins`.

**Cowork.** Open **Customize**, then **Plugins**. Select **Add**, then **Add marketplace**, and enter `wherewolf87/smile-fx-plugins`. Select **SMILE-FX Sales** and **Install**, then connect your tools on its **Connectors** tab. Plugins need a paid Claude plan.

Full steps: [install guide](../README.md#install).

## Try asking

- "Prep me for tomorrow's call with a new referral partner."
- "Summarize this call transcript and draft the follow-up email."
- "Review my pipeline and flag deals with no activity in 14 days."

## First run

Run `/sfx-sales:setup` once. It shows which tools are connected and what each one unlocks, learns how you write, and builds a starter dashboard.

## Skills (36)

Claude uses a skill when your request matches it. You can also call one by name.

| Skill | What it does |
|---|---|
| `/sfx-sales:account-context` | One brief on an account from CRM, email, documents, transcripts and chat. |
| `/sfx-sales:account-plan` | Builds or refreshes an account plan and syncs key fields to the CRM. |
| `/sfx-sales:account-research` | Researches a company or contact: overview, news, likely priorities and fit. |
| `/sfx-sales:account-tiering` | Scores and tiers accounts by fit and engagement so you know where to spend time. |
| `/sfx-sales:call-prep` | Pre-call brief: attendees, history, open opportunity and questions to ask. |
| `/sfx-sales:call-summary` | Turns a transcript or notes into a follow-up email draft, a team summary and CRM updates. |
| `/sfx-sales:close-plan` | Builds the business case and a dated mutual action plan to signature. |
| `/sfx-sales:competitive-intelligence` | Handles a named competitor in a live deal and tracks win and loss patterns. |
| `/sfx-sales:create-an-asset` | Builds a deck or one-pager from your account data and approved materials, with no made-up numbers. |
| `/sfx-sales:crm-hygiene-check` | Read-only audit of CRM opportunities for missing fields, stale dates and stage mismatches. |
| `/sfx-sales:customer-health` | Health check and review prep for a customer account. |
| `/sfx-sales:customer-voice` | Finds attributed customer quotes on a topic across calls and email. |
| `/sfx-sales:daily-briefing` | Morning rundown of meetings, deals closing soon, waiting emails and the day's actions. |
| `/sfx-sales:deal-advance-gap` | Shows what is missing to move one opportunity to the next stage, with owners and dates. |
| `/sfx-sales:deal-review` | Deep review of one opportunity: health, risks, qualification gaps and next actions. |
| `/sfx-sales:deal-signals` | Short alert digest of deals gone quiet, slipping dates and competitor mentions. |
| `/sfx-sales:deal-slip-scenario` | Models the effect on your number if a deal slips, shrinks or is lost. |
| `/sfx-sales:draft-outreach` | Drafts a personal outreach email or sequence and saves it as a draft for review. |
| `/sfx-sales:end-of-day` | Closes the day: calls processed, CRM current, commitments captured, tomorrow planned. |
| `/sfx-sales:expansion-whitespace` | Finds expansion plays in an account or book, with evidence for each. |
| `/sfx-sales:forecast` | Writes the forecast narrative: what is closing, what is at risk and what changed. |
| `/sfx-sales:handle-objection` | Works through an objection using your own win and loss history and customer quotes. |
| `/sfx-sales:inbox-sweep` | Sorts unread customer emails by priority and drafts replies. |
| `/sfx-sales:lead-triage` | Scores and routes inbound leads against your ideal customer profile. |
| `/sfx-sales:log-activity` | Logs a call, meeting or email to the right CRM records when you ask. |
| `/sfx-sales:pipeline-review` | Stage-by-stage pipeline health: coverage, aging, conversion and deals at risk. |
| `/sfx-sales:renewal-radar` | Upcoming renewals with timing, risk and upside. |
| `/sfx-sales:rep-context` | Prep for a one-to-one with a team member: pipeline, activity and where help is needed. |
| `/sfx-sales:route-lead` | Decides who owns an unrouted lead by your rules and drafts the handoff notes. |
| `/sfx-sales:schedule-meeting` | Finds a time, drafts the invite, books it and logs it to the CRM. |
| `/sfx-sales:setup` | First-run setup: checks connected tools, learns your writing style and builds a starter dashboard. |
| `/sfx-sales:stakeholder-map` | Maps the people in a deal: roles, influence, sentiment and who is missing. |
| `/sfx-sales:team-pipeline` | Rolls up a team's pipeline by person and stage and flags deals at risk. |
| `/sfx-sales:update-opportunity` | Guided updates to an opportunity's stage, close date, next steps or amount. |
| `/sfx-sales:weekly-wrap` | End-of-week summary: what closed, what moved, what slipped and what is next. |
| `/sfx-sales:win-loss-review` | Finds patterns in recent wins and losses from CRM data and call transcripts. |

## Connectors

Set up: Slack, HubSpot, Salesforce, Close, monday.com, Clay, ZoomInfo, Notion, Atlassian (Jira, Confluence), Fireflies, Apollo, Outreach, Microsoft 365, Similarweb, Gong, Zoom, Otter.ai, Calendly, Lusha, Crunchbase. Blank on purpose, connect them yourself: Google Calendar, Gmail, Google Drive.

Each connector signs in with your own account, and nothing connects until you do. [CONNECTORS.md](CONNECTORS.md) lists what each one needs.

## Good to know

- Get the consent your state requires before you record any call. Call recorder connectors process everything that is said.
- Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.
- Software suggests. People decide. Check what a skill produces before you use it.

## Credits and licence

Adapted by SMILE-FX P.A. from the `sales` plugin in Anthropic's [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) (commit `da38ec1`), under the Apache License 2.0. SMILE-FX changed the plugin name and metadata, this README, and the connector notes. The changes are listed in [MODIFICATIONS.md](../MODIFICATIONS.md). Licence: [LICENSE](LICENSE). Notices: [NOTICE](../NOTICE).

© 2026 SMILE-FX P.A. SMILE-FX® is a registered trademark of SMILE-FX P.A. SMILE-FX P.A. is not affiliated with, sponsored by or endorsed by Anthropic. Anthropic, Claude, Claude Code and Claude Cowork are trademarks of Anthropic, PBC. They are named here only to describe compatibility.

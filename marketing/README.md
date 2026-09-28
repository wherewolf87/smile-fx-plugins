# SMILE-FX® Marketing

> Plans campaigns, drafts content, checks brand voice, audits SEO and reports on results across your marketing channels.

**Install id:** `sfx-marketing` | **Version:** 1.0.0 | **Skills:** 8 | **Commands:** 0 | **Licence:** Apache-2.0

## Who it is for

Whoever runs marketing for the practice, in house or with an agency.

## Install

**Claude Code.** In a session:

```text
/plugin marketplace add wherewolf87/smile-fx-plugins
/plugin install sfx-marketing@smile-fx-plugins
```

The install command opens the plugin panel so you can review it and pick a scope. From your shell, use `claude plugin marketplace add wherewolf87/smile-fx-plugins` and `claude plugin install sfx-marketing@smile-fx-plugins`.

**Cowork.** Open **Customize**, then **Plugins**, then **Add marketplace**, and enter `wherewolf87/smile-fx-plugins`. Select **SMILE-FX Marketing** and **Install**, then connect your tools on its **Connectors** tab. Plugins need a paid Claude plan.

Full steps: [install guide](../README.md#install).

## Try asking

- "Plan a 30-day campaign to announce our new Saturday hours."
- "Review this newsletter draft against our brand guide."
- "Run an SEO audit of our home page."

## First run

If you keep a brand style guide in your local settings or share it in the conversation, `brand-review` and the drafting skills check against it. Without one, they ask for your voice and audience.

## Skills (8)

Claude uses a skill when your request matches it. You can also call one by name.

| Skill | What it does |
|---|---|
| `/sfx-marketing:brand-review` | Checks content against your brand voice and style guide, with specific before and after fixes. |
| `/sfx-marketing:campaign-plan` | Writes a campaign brief: goals, audience, messages, channels, calendar and success measures. |
| `/sfx-marketing:competitive-brief` | Compares competitor positioning and messaging and finds content gaps. |
| `/sfx-marketing:content-creation` | Drafts content for blogs, social, email newsletters, landing pages and press releases. |
| `/sfx-marketing:draft-content` | Drafts one specific piece with channel formatting, headline options and SEO notes. |
| `/sfx-marketing:email-sequence` | Designs multi-email sequences with copy, timing, branches and exit rules. |
| `/sfx-marketing:performance-report` | Builds a marketing report with key measures, trends, wins, misses and next steps. |
| `/sfx-marketing:seo-audit` | Audits keywords, on-page content, technical issues and competitor gaps. |

## Connectors

Set up: Slack, Canva, Figma, HubSpot, Amplitude (US), Amplitude (EU), Notion, Ahrefs, Similarweb, Klaviyo, Supermetrics. Blank on purpose, connect them yourself: Google Calendar, Gmail.

Each connector signs in with your own account, and nothing connects until you do. [CONNECTORS.md](CONNECTORS.md) lists what each one needs.

## Good to know

- Health care advertising rules apply to anything you publish. Check claims with your compliance lead before posting.
- Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.
- Software suggests. People decide. Check what a skill produces before you use it.

## Credits and licence

Adapted by SMILE-FX P.A. from the `marketing` plugin in Anthropic's [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) (commit `da38ec1`), under the Apache License 2.0. SMILE-FX changed the plugin name and metadata, this README, the connector notes, and skill text that named the old plugin. The changes are listed in [MODIFICATIONS.md](../MODIFICATIONS.md). Licence: [LICENSE](LICENSE). Notices: [NOTICE](../NOTICE).

© 2026 SMILE-FX P.A. SMILE-FX® is a registered trademark of SMILE-FX P.A. SMILE-FX P.A. is not affiliated with, sponsored by or endorsed by Anthropic. Anthropic, Claude, Claude Code and Cowork are trademarks of Anthropic and are named here only to describe compatibility.

# Contributing

Thank you for helping improve SMILE-FX® Plugins. Issues and pull requests are welcome.

## Before you open a pull request

1. Keep skill behaviour the same unless the change fixes a real problem. Say what changed and why.
2. Keep plugin names with the `sfx-` prefix, and keep each marketplace entry's `name` equal to the plugin's `plugin.json` name.
3. Bump `version` in the plugin's `.claude-plugin/plugin.json` for any change users should receive, and add a line to [CHANGELOG.md](CHANGELOG.md).
4. List changed upstream files in [MODIFICATIONS.md](MODIFICATIONS.md).
5. Run the checks below and paste the results in the pull request.

## Checks

```bash
claude plugin validate .                 # the marketplace
claude plugin validate ./marketing       # one plugin; repeat for each folder you changed
```

Every `.json` file must parse. Connector addresses must be full `https://` addresses, or blank on purpose with a note in the plugin's CONNECTORS.md.

## Writing style

Plain words, present tense, short sentences. No superlatives such as "best" or "leading". No em or en dashes: use commas, colons and periods. Name other companies' products only to describe compatibility.

## Health information

Never put real patient information in an issue, pull request, example or test file.

## Licence

This repository is licensed under the Apache License 2.0. By contributing, you agree that your contribution is licensed under the same terms (section 5 of the licence). Keep the NOTICE file and the credit lines.

## Syncing with upstream

The plugins come from Anthropic's [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) at commit `da38ec1`. To take a newer upstream version, compare that commit with the new one for the sixteen folders, apply the changes, keep the SMILE-FX renames, and record the new commit in NOTICE, MODIFICATIONS.md and CHANGELOG.md.

## Moving the repository

The GitHub owner (`wherewolf87`) and the homepage (`https://smile-fx-ai.vercel.app`) appear in the files listed below. If the repository moves to an organization, update each one, then run the checks.

- `.claude-plugin/marketplace.json`
- `customer-support/.claude-plugin/plugin.json`
- `data/.claude-plugin/plugin.json`
- `design/.claude-plugin/plugin.json`
- `engineering/.claude-plugin/plugin.json`
- `enterprise-search/.claude-plugin/plugin.json`
- `finance/.claude-plugin/plugin.json`
- `human-resources/.claude-plugin/plugin.json`
- `legal/.claude-plugin/plugin.json`
- `marketing/.claude-plugin/plugin.json`
- `operations/.claude-plugin/plugin.json`
- `pdf-viewer/.claude-plugin/plugin.json`
- `plugin-builder/.claude-plugin/plugin.json`
- `product-management/.claude-plugin/plugin.json`
- `productivity/.claude-plugin/plugin.json`
- `sales/.claude-plugin/plugin.json`
- `SECURITY.md`
- `small-business/.claude-plugin/plugin.json`
- `CONTRIBUTING.md` (this file)

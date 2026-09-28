# Changelog

All notable changes to SMILE-FX® Plugins. Each plugin's version is in its `.claude-plugin/plugin.json`. Claude Code and Cowork only offer an update when that version changes, so every release bumps it.

## 1.0.0, September 27, 2026

First SMILE-FX release, prepared from Anthropic's [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) at commit `da38ec1` (September 24, 2026).

- 16 plugins, 175 skills and 5 commands, renamed with the `sfx-` prefix under the marketplace name `smile-fx-plugins`.
- `cowork-plugin-management` is now `sfx-plugin-builder`; its skills are `create-plugin` and `customize-plugin`.
- Every plugin version reset to 1.0.0. Upstream versions are recorded in [MODIFICATIONS.md](MODIFICATIONS.md).
- New README for the repository and for each plugin, with skill and command lists counted from the files.
- New CONNECTORS.md with setup notes for every connector. The Definite connector address is left blank because the upstream address returned HTTP 404 on September 27, 2026.
- Apache-2.0 LICENSE in every plugin folder, plus NOTICE, MODIFICATIONS.md, SECURITY.md and CONTRIBUTING.md.
- Not included from upstream: bio-research, the five partner-built plugins, the external marketplace entries and the upstream `.github` automation.

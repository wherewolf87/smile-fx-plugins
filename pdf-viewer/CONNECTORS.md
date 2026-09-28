# Connectors

## How tool references work

This plugin uses one local server on your computer instead of remote connectors.

## Connectors for this plugin

| Category | Server | How it runs |
|---|---|---|
| PDF viewer and annotator | `@modelcontextprotocol/server-pdf@2.0.3` | Local server on your computer, started with `npx` |

Requirements: Node.js 20 or later (the requirement of version 2.0.3), internet access for PDFs opened from a web address, and no account or API key.

## Setup notes

The server runs on your computer. It needs no account and signs in to nothing. Claude Code and Cowork start it when the plugin needs it.

| Connector | Address | What you need | Check on September 27, 2026 | Notes |
|---|---|---|---|---|
| PDF server (local) | `npx -y @modelcontextprotocol/server-pdf@2.0.3 --stdio` | Node.js 20 or later on your computer | Local | Runs on your computer with `npx`. The first run downloads `@modelcontextprotocol/server-pdf` version 2.0.3 from npm. The version is pinned, so a new npm release does not change what runs. Version 2.0.3 requires Node.js 20 or later. No account or API key. |

The full list for all plugins is in [CONNECTORS.md](../CONNECTORS.md) at the repository root.

Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.

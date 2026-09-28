# SMILE-FX® PDF Viewer

> Opens PDFs in an interactive viewer so you can read, annotate, fill forms and place signatures, then download the marked-up copy.

**Install id:** `sfx-pdf-viewer` | **Version:** 1.0.0 | **Skills:** 1 | **Commands:** 4 | **Licence:** Apache-2.0

## Who it is for

Anyone who reviews, fills or signs PDFs.

## Install

**Claude Code.** In a session:

```text
/plugin marketplace add wherewolf87/smile-fx-plugins
/plugin install sfx-pdf-viewer@smile-fx-plugins
```

The install command opens the plugin panel so you can review it and pick a scope. From your shell, use `claude plugin marketplace add wherewolf87/smile-fx-plugins` and `claude plugin install sfx-pdf-viewer@smile-fx-plugins`.

**Cowork.** Open **Customize**, then **Plugins**, then **Add marketplace**, and enter `wherewolf87/smile-fx-plugins`. Select **SMILE-FX PDF Viewer** and **Install**, then connect your tools on its **Connectors** tab. Plugins need a paid Claude plan.

Full steps: [install guide](../README.md#install).

## Try asking

- "Open this vendor agreement PDF."
- "Fill in this supplier application form."
- "Place my initials on page 3."

## Skills (1)

Claude uses a skill when your request matches it. You can also call one by name.

| Skill | What it does |
|---|---|
| `/sfx-pdf-viewer:view-pdf` | Opens a PDF in an interactive viewer for markup, forms and signatures. |

## Commands (4)

| Command | What it does |
|---|---|
| `/sfx-pdf-viewer:annotate` | Proposes markup section by section for you to review in the viewer. |
| `/sfx-pdf-viewer:fill-form` | Fills form fields with a live preview. |
| `/sfx-pdf-viewer:open` | Opens a PDF in the interactive viewer. |
| `/sfx-pdf-viewer:sign` | Places a signature or initials image on a page. |

## Connectors

The PDF server runs on your computer with `npx`. It needs Node.js 20 or later and no account. [CONNECTORS.md](CONNECTORS.md) has the details.

## Good to know

- Do not put patient health information (PHI) into Claude, a plugin or a connected tool unless your Claude plan and every connected service are covered by a signed Business Associate Agreement (BAA). Use de-identified examples when you test.
- Software suggests. People decide. Check what a skill produces before you use it.

## Credits and licence

Adapted by SMILE-FX P.A. from the `pdf-viewer` plugin in Anthropic's [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) (commit `da38ec1`), under the Apache License 2.0. SMILE-FX changed the plugin name and metadata, this README, the connector notes, and skill text that named the old plugin. The changes are listed in [MODIFICATIONS.md](../MODIFICATIONS.md). Licence: [LICENSE](LICENSE). Notices: [NOTICE](../NOTICE).

© 2026 SMILE-FX P.A. SMILE-FX® is a registered trademark of SMILE-FX P.A. SMILE-FX P.A. is not affiliated with, sponsored by or endorsed by Anthropic. Anthropic, Claude, Claude Code and Cowork are trademarks of Anthropic and are named here only to describe compatibility.

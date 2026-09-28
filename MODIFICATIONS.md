# Modifications

This file states how SMILE-FX® Plugins differs from the work it adapts, as section 4(b) of the Apache License 2.0 requires. It is generated from a byte-for-byte comparison with the upstream snapshot.

- Upstream: [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins), commit `da38ec1ee89d41e5380e652a97382695003396e7` (September 24, 2026).
- Modified by: SMILE-FX P.A., September 2026.
- Changed Markdown skill and reference files also carry a comment at the top that says SMILE-FX modified them.

## Repository level

| File | Change |
|---|---|
| `LICENSE` | Clean Apache License 2.0 text, identical to the per-plugin LICENSE files upstream and to the text at apache.org. The 10 lines of non-licence text added to the upstream root LICENSE by upstream pull request #193 are not carried over. |
| `.claude-plugin/marketplace.json` | New file replacing the upstream marketplace. Name `smile-fx-plugins` (the upstream name is reserved for Anthropic). Lists only the 16 plugins below; upstream listed 121. |
| `README.md`, `CONNECTORS.md`, `NOTICE`, `MODIFICATIONS.md`, `CHANGELOG.md`, `SECURITY.md`, `CONTRIBUTING.md` | New SMILE-FX files. |
| `assets/` | SMILE-FX® logo files for the README. Not licensed under the Apache License. |

## Not included from upstream

- `bio-research`: outside the audience; uses research connectors.
- `partner-built/` (apollo, brand-voice, common-room, slack, zoom-plugin): built and owned by other companies.
- The 99 external marketplace entries: other companies' repositories.
- `.github/` automation: upstream CI that depends on Anthropic accounts.

## Plugin level

### small-business/ (`sfx-small-business`, upstream `small-business`)

| File | Change |
|---|---|
| `small-business/.claude-plugin/plugin.json` | renamed `small-business` to `sfx-small-business`; display name "SMILE-FX Small Business"; new description, author (SMILE-FX), homepage, repository, licence and keywords; version reset from 1.35.1 to 1.0.0 |
| `small-business/README.md` | rewritten: SMILE-FX install steps, skill and command lists counted from the files, connector notes, health data note, credits |
| `small-business/shared/connector-call-shapes.md` | connector registration name `small-business:<server>` renamed to `sfx-small-business:<server>`; tool name prefix `mcp__plugin_small-business_` renamed to `mcp__plugin_sfx-small-business_`; SMILE-FX modification notice added |
| `small-business/shared/connector-neutrality.md` | connector registration name `small-business:<server>` renamed to `sfx-small-business:<server>`; tool name prefix `mcp__plugin_small-business_` renamed to `mcp__plugin_sfx-small-business_`; wording "Anthropic's positioning for the plugin" changed to "the plugin's positioning"; SMILE-FX modification notice added |
| `small-business/skills/build-connector/reference/discovery.md` | connector registration name `small-business:<server>` renamed to `sfx-small-business:<server>`; SMILE-FX modification notice added |
| `small-business/skills/growth-pulse/reference/data_sources.md` | connector registration name `small-business:<server>` renamed to `sfx-small-business:<server>`; SMILE-FX modification notice added |
| `small-business/skills/month-end-prep/reference/xero-reconcile.md` | connector registration name `small-business:<server>` renamed to `sfx-small-business:<server>`; SMILE-FX modification notice added |
| `small-business/skills/month-end-prep/reference/zoho-books-reconcile.md` | connector registration name `small-business:<server>` renamed to `sfx-small-business:<server>`; SMILE-FX modification notice added |
| `small-business/skills/smb-onboard/reference/onboard-checklist.md` | connector registration name `small-business:<server>` renamed to `sfx-small-business:<server>`; SMILE-FX modification notice added |
| `small-business/skills/smb-onboard/SKILL.md` | connector registration name `small-business:<server>` renamed to `sfx-small-business:<server>`; SMILE-FX modification notice added |
| `small-business/skills/smb-router/reference/connector-map.md` | connector registration name `small-business:<server>` renamed to `sfx-small-business:<server>`; SMILE-FX modification notice added |
| `small-business/skills/smb-router/SKILL.md` | connector registration name `small-business:<server>` renamed to `sfx-small-business:<server>`; SMILE-FX modification notice added |
| `small-business/CONNECTORS.md` | added |
| `small-business/LICENSE` | added (copy of the Apache License 2.0) |

All other files in this folder are unchanged from upstream.

### marketing/ (`sfx-marketing`, upstream `marketing`)

| File | Change |
|---|---|
| `marketing/.claude-plugin/plugin.json` | renamed `marketing` to `sfx-marketing`; display name "SMILE-FX Marketing"; new description, author (SMILE-FX), homepage, repository, licence and keywords; version reset from 1.2.0 to 1.0.0 |
| `marketing/CONNECTORS.md` | intro rewritten; category table corrected to match `.mcp.json` (placeholders unchanged); setup notes added for every connector |
| `marketing/README.md` | rewritten: SMILE-FX install steps, skill and command lists counted from the files, connector notes, health data note, credits |

All other files in this folder are unchanged from upstream.

### sales/ (`sfx-sales`, upstream `sales`)

| File | Change |
|---|---|
| `sales/.claude-plugin/plugin.json` | renamed `sales` to `sfx-sales`; display name "SMILE-FX Sales"; new description, author (SMILE-FX), homepage, repository, licence and keywords; version reset from 2.0.1 to 1.0.0 |
| `sales/CONNECTORS.md` | intro rewritten; category table corrected to match `.mcp.json` (placeholders unchanged); setup notes added for every connector |
| `sales/README.md` | rewritten: SMILE-FX install steps, skill and command lists counted from the files, connector notes, health data note, credits |

All other files in this folder are unchanged from upstream.

### customer-support/ (`sfx-customer-support`, upstream `customer-support`)

| File | Change |
|---|---|
| `customer-support/.claude-plugin/plugin.json` | renamed `customer-support` to `sfx-customer-support`; display name "SMILE-FX Customer Support"; new description, author (SMILE-FX), homepage, repository, licence and keywords; version reset from 1.3.0 to 1.0.0 |
| `customer-support/CONNECTORS.md` | intro rewritten; category table corrected to match `.mcp.json` (placeholders unchanged); setup notes added for every connector |
| `customer-support/README.md` | rewritten: SMILE-FX install steps, skill and command lists counted from the files, connector notes, health data note, credits |

All other files in this folder are unchanged from upstream.

### operations/ (`sfx-operations`, upstream `operations`)

| File | Change |
|---|---|
| `operations/.claude-plugin/plugin.json` | renamed `operations` to `sfx-operations`; display name "SMILE-FX Operations"; new description, author (SMILE-FX), homepage, repository, licence and keywords; version reset from 1.3.0 to 1.0.0 |
| `operations/CONNECTORS.md` | intro rewritten; category table corrected to match `.mcp.json` (placeholders unchanged); setup notes added for every connector |
| `operations/README.md` | rewritten: SMILE-FX install steps, skill and command lists counted from the files, connector notes, health data note, credits |
| `operations/LICENSE` | added (copy of the Apache License 2.0) |

All other files in this folder are unchanged from upstream.

### finance/ (`sfx-finance`, upstream `finance`)

| File | Change |
|---|---|
| `finance/.claude-plugin/plugin.json` | renamed `finance` to `sfx-finance`; display name "SMILE-FX Finance"; new description, author (SMILE-FX), homepage, repository, licence and keywords; version reset from 1.3.0 to 1.0.0 |
| `finance/CONNECTORS.md` | intro rewritten; category table corrected to match `.mcp.json` (placeholders unchanged); setup notes added for every connector |
| `finance/README.md` | rewritten: SMILE-FX install steps, skill and command lists counted from the files, connector notes, health data note, credits |

All other files in this folder are unchanged from upstream.

### human-resources/ (`sfx-human-resources`, upstream `human-resources`)

| File | Change |
|---|---|
| `human-resources/.claude-plugin/plugin.json` | renamed `human-resources` to `sfx-human-resources`; display name "SMILE-FX Human Resources"; new description, author (SMILE-FX), homepage, repository, licence and keywords; version reset from 1.3.0 to 1.0.0 |
| `human-resources/CONNECTORS.md` | intro rewritten; category table corrected to match `.mcp.json` (placeholders unchanged); setup notes added for every connector |
| `human-resources/README.md` | rewritten: SMILE-FX install steps, skill and command lists counted from the files, connector notes, health data note, credits |
| `human-resources/LICENSE` | added (copy of the Apache License 2.0) |

All other files in this folder are unchanged from upstream.

### productivity/ (`sfx-productivity`, upstream `productivity`)

| File | Change |
|---|---|
| `productivity/.claude-plugin/plugin.json` | renamed `productivity` to `sfx-productivity`; display name "SMILE-FX Productivity"; new description, author (SMILE-FX), homepage, repository, licence and keywords; version reset from 1.3.1 to 1.0.0 |
| `productivity/CONNECTORS.md` | intro rewritten; category table corrected to match `.mcp.json` (placeholders unchanged); setup notes added for every connector |
| `productivity/README.md` | rewritten: SMILE-FX install steps, skill and command lists counted from the files, connector notes, health data note, credits |
| `productivity/skills/memory-management/SKILL.md` | slash command namespace renamed (for example `/productivity:start` to `/sfx-productivity:start`); SMILE-FX modification notice added |
| `productivity/skills/start/SKILL.md` | slash command namespace renamed (for example `/productivity:start` to `/sfx-productivity:start`); SMILE-FX modification notice added |
| `productivity/skills/task-management/SKILL.md` | slash command namespace renamed (for example `/productivity:start` to `/sfx-productivity:start`); SMILE-FX modification notice added |
| `productivity/skills/update/SKILL.md` | slash command namespace renamed (for example `/productivity:start` to `/sfx-productivity:start`); SMILE-FX modification notice added |

All other files in this folder are unchanged from upstream.

### legal/ (`sfx-legal`, upstream `legal`)

| File | Change |
|---|---|
| `legal/.claude-plugin/plugin.json` | renamed `legal` to `sfx-legal`; display name "SMILE-FX Legal"; new description, author (SMILE-FX), homepage, repository, licence and keywords; version reset from 1.3.0 to 1.0.0 |
| `legal/CONNECTORS.md` | intro rewritten; category table corrected to match `.mcp.json` (placeholders unchanged); setup notes added for every connector |
| `legal/README.md` | rewritten: SMILE-FX install steps, skill and command lists counted from the files, connector notes, health data note, credits |

All other files in this folder are unchanged from upstream.

### data/ (`sfx-data`, upstream `data`)

| File | Change |
|---|---|
| `data/.claude-plugin/plugin.json` | renamed `data` to `sfx-data`; display name "SMILE-FX Data"; new description, author (SMILE-FX), homepage, repository, licence and keywords; version reset from 1.1.0 to 1.0.0 |
| `data/.mcp.json` | Definite connector address set to blank (the upstream address returned HTTP 404 on September 27, 2026) |
| `data/CONNECTORS.md` | intro rewritten; category table corrected to match `.mcp.json` (placeholders unchanged); setup notes added for every connector |
| `data/README.md` | rewritten: SMILE-FX install steps, skill and command lists counted from the files, connector notes, health data note, credits |

All other files in this folder are unchanged from upstream.

### design/ (`sfx-design`, upstream `design`)

| File | Change |
|---|---|
| `design/.claude-plugin/plugin.json` | renamed `design` to `sfx-design`; display name "SMILE-FX Design"; new description, author (SMILE-FX), homepage, repository, licence and keywords; version reset from 1.2.0 to 1.0.0 |
| `design/CONNECTORS.md` | intro rewritten; category table corrected to match `.mcp.json` (placeholders unchanged); setup notes added for every connector |
| `design/README.md` | rewritten: SMILE-FX install steps, skill and command lists counted from the files, connector notes, health data note, credits |
| `design/LICENSE` | added (copy of the Apache License 2.0) |

All other files in this folder are unchanged from upstream.

### enterprise-search/ (`sfx-enterprise-search`, upstream `enterprise-search`)

| File | Change |
|---|---|
| `enterprise-search/.claude-plugin/plugin.json` | renamed `enterprise-search` to `sfx-enterprise-search`; display name "SMILE-FX Enterprise Search"; new description, author (SMILE-FX), homepage, repository, licence and keywords; version reset from 1.3.0 to 1.0.0 |
| `enterprise-search/CONNECTORS.md` | intro rewritten; category table corrected to match `.mcp.json` (placeholders unchanged); setup notes added for every connector |
| `enterprise-search/README.md` | rewritten: SMILE-FX install steps, skill and command lists counted from the files, connector notes, health data note, credits |

All other files in this folder are unchanged from upstream.

### product-management/ (`sfx-product-management`, upstream `product-management`)

| File | Change |
|---|---|
| `product-management/.claude-plugin/plugin.json` | renamed `product-management` to `sfx-product-management`; display name "SMILE-FX Product Management"; new description, author (SMILE-FX), homepage, repository, licence and keywords; version reset from 1.2.0 to 1.0.0 |
| `product-management/CONNECTORS.md` | intro rewritten; category table corrected to match `.mcp.json` (placeholders unchanged); setup notes added for every connector |
| `product-management/README.md` | rewritten: SMILE-FX install steps, skill and command lists counted from the files, connector notes, health data note, credits |

All other files in this folder are unchanged from upstream.

### pdf-viewer/ (`sfx-pdf-viewer`, upstream `pdf-viewer`)

| File | Change |
|---|---|
| `pdf-viewer/.claude-plugin/plugin.json` | renamed `pdf-viewer` to `sfx-pdf-viewer`; display name "SMILE-FX PDF Viewer"; new description, author (SMILE-FX), homepage, repository, licence and keywords; version reset from 0.2.0 to 1.0.0 |
| `pdf-viewer/commands/annotate.md` | slash command namespace renamed (for example `/productivity:start` to `/sfx-productivity:start`); SMILE-FX modification notice added |
| `pdf-viewer/commands/fill-form.md` | slash command namespace renamed (for example `/productivity:start` to `/sfx-productivity:start`); SMILE-FX modification notice added |
| `pdf-viewer/commands/sign.md` | slash command namespace renamed (for example `/productivity:start` to `/sfx-productivity:start`); SMILE-FX modification notice added |
| `pdf-viewer/CONNECTORS.md` | intro rewritten; category table corrected to match `.mcp.json` (placeholders unchanged); setup notes added for every connector |
| `pdf-viewer/README.md` | rewritten: SMILE-FX install steps, skill and command lists counted from the files, connector notes, health data note, credits |

All other files in this folder are unchanged from upstream.

### engineering/ (`sfx-engineering`, upstream `engineering`)

| File | Change |
|---|---|
| `engineering/.claude-plugin/plugin.json` | renamed `engineering` to `sfx-engineering`; display name "SMILE-FX Engineering"; new description, author (SMILE-FX), homepage, repository, licence and keywords; version reset from 1.2.0 to 1.0.0 |
| `engineering/CONNECTORS.md` | intro rewritten; category table corrected to match `.mcp.json` (placeholders unchanged); setup notes added for every connector |
| `engineering/README.md` | rewritten: SMILE-FX install steps, skill and command lists counted from the files, connector notes, health data note, credits |
| `engineering/LICENSE` | added (copy of the Apache License 2.0) |

All other files in this folder are unchanged from upstream.

### plugin-builder/ (`sfx-plugin-builder`, upstream `cowork-plugin-management`)

Folder renamed from `cowork-plugin-management/` to `plugin-builder/`.

| File | Change |
|---|---|
| `plugin-builder/.claude-plugin/plugin.json` | renamed `cowork-plugin-management` to `sfx-plugin-builder`; display name "SMILE-FX Plugin Builder"; new description, author (SMILE-FX), homepage, repository, licence and keywords; version reset from 0.2.2 to 1.0.0 |
| `plugin-builder/skills/create-plugin/references/component-schemas.md` | moved from `cowork-plugin-management/skills/create-cowork-plugin/references/component-schemas.md`; skill renamed without "Cowork" (`create-cowork-plugin` to `create-plugin`, `cowork-plugin-customizer` to `customize-plugin`) and title changed to match; SMILE-FX modification notice added |
| `plugin-builder/skills/create-plugin/SKILL.md` | moved from `cowork-plugin-management/skills/create-cowork-plugin/SKILL.md`; skill renamed without "Cowork" (`create-cowork-plugin` to `create-plugin`, `cowork-plugin-customizer` to `customize-plugin`) and title changed to match; SMILE-FX modification notice added |
| `plugin-builder/skills/customize-plugin/SKILL.md` | moved from `cowork-plugin-management/skills/cowork-plugin-customizer/SKILL.md`; skill renamed without "Cowork" (`create-cowork-plugin` to `create-plugin`, `cowork-plugin-customizer` to `customize-plugin`) and title changed to match; SMILE-FX modification notice added |
| `plugin-builder/README.md` | added |
| `plugin-builder/LICENSE` | moved from `cowork-plugin-management/LICENSE`, content unchanged |
| `plugin-builder/skills/create-plugin/references/example-plugins.md` | moved from `cowork-plugin-management/skills/create-cowork-plugin/references/example-plugins.md`, content unchanged |
| `plugin-builder/skills/customize-plugin/examples/customized-mcp.json` | moved from `cowork-plugin-management/skills/cowork-plugin-customizer/examples/customized-mcp.json`, content unchanged |
| `plugin-builder/skills/customize-plugin/LICENSE.txt` | moved from `cowork-plugin-management/skills/cowork-plugin-customizer/LICENSE.txt`, content unchanged |
| `plugin-builder/skills/customize-plugin/references/mcp-servers.md` | moved from `cowork-plugin-management/skills/cowork-plugin-customizer/references/mcp-servers.md`, content unchanged |
| `plugin-builder/skills/customize-plugin/references/search-strategies.md` | moved from `cowork-plugin-management/skills/cowork-plugin-customizer/references/search-strategies.md`, content unchanged |

All other files in this folder are unchanged from upstream.

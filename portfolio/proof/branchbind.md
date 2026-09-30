# BranchBind — public proof

**Purpose:** Save the exact ChatGPT conversation branch currently being viewed as Markdown, to GitHub, the browser download location, or both.

This is sanitized proof from the current private BranchBind source. No archive credentials, Worker keys, conversation contents, or private service URLs are included.

## Real output

BranchBind writes filenames in this form:

```text
bb--<project-or-no-project>--<conversation-slug>.md
```

Example from the documented current behavior:

```text
bb--ai-unfuck--dev-nav-d.md
```

## Current Chrome extension boundary

The current Manifest V3 source declares:

```json
{
  "name": "BranchBind",
  "version": "1.0.0",
  "permissions": ["activeTab", "scripting", "downloads"]
}
```

The extension uses the authenticated ChatGPT page context to load conversation data and reconstructs the active path from `current_node`, rather than flattening sibling branches that are not part of the conversation the user is viewing.

The action row is intentionally small:

- **GitHub + Download**
- **GitHub**
- **Download**

GitHub archive writes go through a narrow server-side Worker boundary; a broad GitHub token is not embedded in the extension.

## Verification

Current source was read directly from `donzpixelz/branchbind` on 2026-09-30.

- Manifest: `manifest.json`
- Main documentation: `README.md`
- Current `main` commit at verification: `99bd18f9037e9b8d541baf4928baf6fb501a3dd2`

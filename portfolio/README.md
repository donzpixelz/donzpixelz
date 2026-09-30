# Automation & AI Systems

**Donald (Chip) Wilson** — automation, integrations, browser tooling, and AI-assisted implementation

I build practical systems that make messy technical work easier to run, inspect, and trust.

**Tools I work across:** `n8n` · `REST APIs` · `Webhooks` · `Chrome extensions` · `Swift / AppKit` · `Cloudflare Workers / D1 / R2` · `TypeScript` · `Google Ads API / GAQL` · `GitHub`

---

## Featured work

### 1. BranchBind

**Save the exact ChatGPT conversation branch you are looking at and preserve it cleanly to GitHub or download it.**

BranchBind is a focused Chrome extension I use for current conversation preservation. It reconstructs the active branch instead of mixing in abandoned sibling branches, then exports clean Markdown.

**Real output**

```text
bb--ai-unfuck--dev-nav-d.md
```

| | |
| --- | --- |
| **Built with** | Chrome MV3 · JavaScript · authenticated page-context requests · Cloudflare Worker · GitHub |
| **Used for** | Current-branch ChatGPT export, browser download, canonical archive |
| **Proof** | [Current sanitized BranchBind proof →](./proof/branchbind.md) |

---

### 2. PageShot

**Make full-page and responsive Chrome screenshots easy during web development and AI-assisted review.**

PageShot is a native macOS utility with three simple actions:

```text
Active Tab        → capture the entire active Chrome page
Quick Test        → 430×900 + 1440×900
Full Responsive   → eight full-page viewport captures
```

The interface and capture engines are real working source, including the intentional Jax/LoLo branding.

| | |
| --- | --- |
| **Built with** | Swift / AppKit · AppleScript · Chrome DevTools · macOS Accessibility |
| **Used for** | Full-page capture, responsive QA, getting screenshots back into the human/AI review loop |
| **Proof** | [Current sanitized PageShot proof →](./proof/pageshot.md) |

---

### 3. Conversation Export — Canonical

**Take an exact request, resolve the correct conversation, export it, and verify the requested result instead of merely trusting that the workflow ran.**

This is a live n8n/API workflow with fail-closed identity handling and real execution history.

**Verified execution**

```text
status:                 success
trigger:                webhook
conversation turns:     384
markdown bytes:         268,184
full branch to root:    confirmed
```

| | |
| --- | --- |
| **Built with** | n8n · Webhooks · REST APIs · JSON · authenticated routing · verification |
| **Used for** | Exact conversation resolution and verified export |
| **Proof** | [Sanitized runtime execution →](./proof/conversation-export-run.json) |

---

### 4. TrafficMonitor

**See real website visitor/session behavior and preserve trustworthy paid-traffic attribution.**

TrafficMonitor is a first-party production system for understanding visitor sessions without rewriting the evidence later. It keeps original paid-traffic attribution intact while allowing later sessions and repeat paid clicks to be analyzed separately.

**What it preserves**

```text
first touch       → immutable visitor attribution
repeat paid click → session-level attribution
current Ads state → separate from historical evidence
```

| | |
| --- | --- |
| **Built with** | Cloudflare Workers · D1 · R2 · TypeScript · Google Ads API / GAQL |
| **Used for** | Visitor/session behavior, attribution, live operational review, historical evidence |
| **Proof** | [Sanitized production-system evidence →](./proof/traffic-attribution-system.md) |

---

## More work

| Project / system | What it does |
| --- | --- |
| **Customer Intake / Human Review** | Captures a technical problem with low friction, delivers it server-side, and keeps diagnosis/scope decisions human-controlled. [Proof →](./proof/customer-intake-system.md) |
| **Codex Launcher / controlled task execution** | Turns one exact implementation request into a controlled AI task with explicit context, permissions, result capture, and verification. |
| **ChatGPT Project & Conversation tooling** | Exact-ID project/conversation operations with ambiguity rejection, readback, and archive behavior. |
| **Evidence-gated process analysis** | Research and qualification workflows that establish real friction before treating a manual process as an automation target. |

---

## What I can step into

`n8n workflows` · `API/webhook integrations` · `workflow repair` · `browser tooling` · `Cloudflare systems` · `Google Ads data` · `testing & verification` · `technical handoff`

> **AI-assisted implementation:** AI is used heavily for implementation; Chip owns requirements, architecture, testing, verification, acceptance, and handoff.

---

[LinkedIn](https://www.linkedin.com/in/donzpixelz/) · [GitHub](https://github.com/donzpixelz) · [Unjank AI](https://unjankai.com/)

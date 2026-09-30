# PageShot — public proof

**Purpose:** Make full-page and responsive Chrome screenshots easy during web development and AI-assisted review.

This is sanitized proof from the reconciled PageShot source. No private browser data or captured customer/site content is included.

## Actual application controls

The current native macOS application builds these three capture actions directly in its Swift/AppKit interface:

```text
Active Tab
Quick Test
Full Responsive Test
```

### Active Tab

Captures the entire currently active Chrome tab at its current viewport and saves the image to the macOS Desktop.

### Quick Test

Captures two full-page screenshots:

```text
430 × 900
1440 × 900
```

### Full Responsive Test

Captures eight full-page screenshots:

```text
320 × 568
390 × 844
430 × 900
768 × 1024
1024 × 768
1280 × 800
1440 × 900
1920 × 1080
```

## Real implementation boundary

- Native interface: Swift / AppKit
- Chrome automation: AppleScript
- Full-page capture: Chrome DevTools **Capture full size screenshot**
- Responsive sizing: Chrome JavaScript from Apple Events
- UI automation: macOS Accessibility APIs
- Intentional application branding: Jax/LoLo assets are part of the current source tree

The generated `PageShot.app` bundle is intentionally not committed; the repository preserves source, assets, capture engines, and the build workflow.

## Verification

PageShot reconciliation and documentation are complete.

- Repository: `donzpixelz/pageshot`
- Current `main` commit at verification: `0a63ba30dd857b316f3f3f59ea679703df0ac465`
- Documentation commit message: `Document PageShot project and build workflow`

[README.md](https://github.com/user-attachments/files/30091466/README.md)
# ⚠️ TEST AREA ONLY — NOT PRODUCTION READY ⚠️

**This repository is an experimental prototype space for exploring how the CfA
Design System could be implemented in code. Nothing in here is approved,
finalized, or safe to use in a real product.**

- Not accessibility-audited to a shippable standard
- Not cross-browser tested
- Not reviewed by the design system team
- Colors, tokens, and markup may change or be thrown out entirely
- Do not copy this code into a production project

If you're looking for the real, approved design system, this is not it —
check with the design system team for the current source of truth.

---

## What's actually in here

An early, in-progress vanilla HTML/CSS implementation of the **Primary button**
component from the CfA Design System Figma file, used to test whether a
framework-agnostic, token-based approach (CSS custom properties, no build
step, no JavaScript) is a viable direction — see `components/button/`.

**Current scope:**
- Primary button style only (Secondary/Tertiary not started)
- All interactive states: default, hover, active, focus, disabled
- Both sizes (regular, small), icon-left/right placement
- Default theme only — dark mode and the "simplefile" theme are intentionally
  not implemented yet
- Icons are generic placeholder SVGs, not the real Figma icon assets

**Known open issues:**
- Default and Hover backgrounds don't meet the 3:1 non-text contrast minimum
  against a white page — flagged, not yet fixed
- Cross-browser testing so far has surfaced real differences between Chrome
  and Safari that are still being worked through

## Viewing it locally

```bash
npx serve
```
Then open the printed `localhost` URL and navigate to `components/button/`.
(Opening the HTML file directly by double-clicking it can behave differently
across browsers — Safari in particular restricts loading CSS across parent
directories over `file://` — so always view it through a local server.)

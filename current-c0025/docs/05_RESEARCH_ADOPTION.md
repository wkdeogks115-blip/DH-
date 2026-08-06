# C0025 RESEARCH ADOPTION

## nextlevelbuilder/ui-ux-pro-max-skill

Adopted as a broad heuristic and checklist source:

- small brand palette,
- neutral and semantic color separation,
- one primary action per screen,
- consistent focus, elevation and dark-mode behavior,
- documented contrast checks.

Not adopted as the final color authority because its example palettes and ratio rules are generic and product-type driven.

## Stronger primary references

- `radix-ui/colors`: useful for predictable scales, dark variants and alpha variants.
- `primer/primitives`: useful for primitive → functional → component token architecture and color modes.
- `uswds/uswds`: useful for theme, state and system token separation plus accessibility guidance.
- `adobe/spectrum-design-data`: useful for token manifests, validation and diff tooling.

C0025 uses these architectural ideas without importing their packages or copying a full foreign palette.

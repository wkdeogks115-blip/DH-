# C0025 COLOR TOKEN CONTRACT

## Architecture

1. Primitive tokens define stable neutral, cyan and status values.
2. Semantic tokens describe roles such as canvas, surface, text, border, action and state.
3. Component rules consume semantic roles only.
4. Legacy aliases map older variable names to the semantic contract during migration.

## Usage rules

- Cyan is reserved for the main action, focus and selected state.
- Neutral surfaces carry page and card hierarchy.
- Success, warning and danger colors communicate state only.
- A color must not be the only carrier of meaning.
- Normal text pairs must meet at least 4.5:1.
- Interactive boundaries targeted by this Candidate must meet at least 3:1 against the adjacent surface.
- Raw color literals may appear in the primitive declaration block, not in component declarations.

<img width="1080" height="922" alt="preview" src="https://github.com/user-attachments/assets/d955640c-582b-458f-810b-28082c25885c" />
# OpenShapes v1.2

A CC0 controller glyph pack featuring **individual, editable SVGs** in
**filled (bold)** and **outlined (lightweight)** styles.

## Content
- `svg/filled/colour`, `svg/filled/white`, `svg/filled/black`
- `svg/outlined/colour`, `svg/outlined/white`, `svg/outlined/black`
- `mappings/sdl3.json`: exact SDL3 button/axis key names -> filenames.
- `mappings/steam-input-guide.json`: semantic reference for Steam Input integrations, not official Valve enum constants.
- `preview.png`: all designs at a glance.

Each SVG has a `viewBox="0 0 100 100"` and uses `currentColor` for recolouring,
with the palette preset via a root style attribute.

**Filled and outlined:** both use the same shape geometry. The filled edition
uses bolder strokes; the outlined edition uses slimmer strokes. Open negative
space remains in Gate, Peak, Fork and Halo, by design.

**Symbols:** Gate=west, Peak=north, Fork=south, Halo=east.
The meaning tags context/secondary/cancel/confirm are *suggestions*, not
hard-coded game actions. Use actual player bindings to select prompts.

**D-pad:** a solid plus-shaped full D-pad, with separate arrow glyphs for
cardinal and diagonal movements.

**L3 and R3 are the left and right stick clicks**, not separate controls.
L2/R2 represent analog trigger axes. L4/L5 and R4/R5 represent rear paddles,
only where the device exposes them.

**Steam Input:** Steam Input action origins are device-dependent; the mapping
guide is intentionally conceptual, rather than falsely presenting an
all-purpose direct mapping. `home` may be reserved by the host operating system.

**Manufacturing:** All icon labels (L1–L5, R1–R5, MISC2–MISC6) are pure SVG vector paths. No embedded text nodes, external fonts or font-family dependencies remain. Text was outlined from DejaVu Sans Bold (see `FONT-ATTRIBUTION.md`).

**Scalability:** SVG is resolution-independent, but legibility of fine details,
especially two-character labels below 16 px, still needs visual testing.
All geometry is centred within the same 100×100 viewBox.

## License
CC0 1.0 Universal. See `LICENSE`. Third-party IP clearance is not guaranteed.

## Technical references
- SDL3 gamepad buttons: https://wiki.libsdl.org/SDL3/SDL_GamepadButton
- SDL3 axes: https://wiki.libsdl.org/SDL3/SDL_GamepadAxis
- Steam Input: https://partner.steamgames.com/doc/features/steam_controller

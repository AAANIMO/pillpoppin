# Usage

## The idea

Pillpoppin treats the raw bytes of your image as an audio signal. Audio effects
that would warp a sound — gain, compression, distortion, pitch shift, delay,
reverb, EQ — instead warp the *pixels*, producing controlled databending glitch.

## Layout

- **Monitor** (top-left) — BEFORE and AFTER previews, plus a compact waveform of
  the image-as-audio and the control bar (APPLY, OVERDOSE, undo/redo).
- **Effects chain** (bottom-left) — the ordered stack of effects currently
  applied. Always visible, scrolls internally.
- **Add effect** (right rail) — the effect palette, grouped by category.

## Workflow

1. **Load an image** — PNG, JPG or TIFF.
2. **Add effects** from the right rail. Categories:
   - **VOLUME / COMP** — gain, threshold/ratio compression, ceiling.
   - **FADING** — fade in / out over a length of the signal.
   - **PITCH / TEMPO** — semitone shift, time-stretch.
   - **EQ / FILTERS** — bass / mid / treble shaping.
   - **DELAY / REVERB** — echoes and space.
   - **DIST / MOD** — distortion and modulation.
   - **CORE** — invert, reverse and other base operations.
3. **Tune parameters** — the AFTER preview re-processes automatically (no button
   to press). Reorder or toggle effects in the chain to taste.
4. **APPLY** — bakes the current chain into the image as a new layer, so you can
   build further passes on top. This is the only explicit commit action.
5. **OVERDOSE** — the "go too far" button: pushes the chain hard for maximum
   damage. It asks for confirmation first.
6. **Undo / Redo** — step back and forth through your edits.
7. **Export** — save as PNG, JPG or TIFF.

## Tips

- Small parameter nudges compound after several APPLY passes — build gradually.
- OVERDOSE is destructive by design; APPLY first if you want to keep a clean base.

# Changelog

## 1.44.0 — Nov 17, 2026

Typing responsiveness, rebuilt:

- **Keys type on touch-down.** A letter now lands the moment your finger
  touches the key — iPhone-style — instead of waiting for the release.
  Lifting your finger slightly off the key, or racing to the next one,
  can no longer swallow a tap, so fast typing stops dropping letters.
- **Bigger, smarter hit targets.** Taps that land in the gaps between
  keys are no longer lost: they go to the nearest key, and the key the
  dictionary predicts you want next gets a wider invisible target —
  the same dynamic hit-area trick the iPhone keyboard uses.
- **Snappier suggestions.** The suggestion strip no longer recalculates
  on every single keystroke, so it can't slow your typing down.

## 1.43.0 — Nov 16, 2026

Key press effects, rebuilt:

- **Animated key preview.** The letter bubble above a pressed key now
  grows out of the key — it scales up with a soft overshoot and settles,
  then fades out instead of snapping off. Press the next key and the
  previous bubble fades away as the new one appears.
- **No more preview lag.** The preview used to open a separate system
  window on every keypress, which is what made it feel delayed. It now
  renders inside the keyboard itself, in the same frame as your tap.
- **Full-color key highlight.** A pressed key now fills completely with
  your accent color while your finger is on it (the letter flips to a
  readable color on top), instead of lightening by one shade. When you
  lift your finger, the color slowly melts back over about half a
  second — so you can still see which letter you pressed last.
- The new highlight applies to both the **Popup** and **Highlight**
  key press effects (Settings → Key press effect).

## 1.42.0 — Nov 15, 2026

First release published on GitHub:

- Voice typing with your own OpenAI key (Whisper dictation with smart
  formatting), Fix & Continue on gpt-4o-mini
- Keyless GIF search, clipboard history (up to 50, secrets never
  stored), emoji panel
- Languages on demand: English built in, Russian and Hebrew bundled,
  11 more languages downloadable (~1 MB each, then fully offline)
- Accent theme packs, photo background with blur and dim, key text
  color, optional number row, symbols on letter keys (long-press)
- Personal dictionary that learns your words, context-aware
  suggestions and typo corrections

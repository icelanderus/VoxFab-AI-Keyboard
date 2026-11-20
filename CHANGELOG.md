# Changelog

## 1.66.0 — Nov 20, 2026

- **Continue is gone.** The Continue button was removed from the
  toolbar — it suggested a continuation in the suggestion strip
  instead of typing it, which mostly confused people. Fix stays.
- **English is the only built-in language.** Russian and Hebrew are
  optional downloads now, exactly like every other language: their
  bundled dictionaries and context tables (~3.5 MB of data) no longer
  ship inside the app, and a fresh install starts with English only.
  If Russian or Hebrew were already enabled on your phone, their
  dictionaries download automatically in the background once — no
  action needed.
- **A NEW badge you can actually read.** The tiny UPDATE badge on the
  Settings icon is now a big green NEW pill sitting over the icon.
- **Panel headers, fixed.** The back arrow in the emoji / GIF /
  clipboard panels is a proper bold arrow (it used to be a thin text
  glyph), and the emoji panel's delete key is a clean outline icon
  instead of a stark white blob.
- **The letter fades with the key.** When a pressed key's glow melts
  back, its letter now fades along with the fill instead of popping
  back in one frame.

## 1.61.0 — Nov 19, 2026

- **Mic sounds, rewritten low and muted.** Every built-in mic on/off
  sound was regenerated an octave lower with a heavy low-pass filter —
  soft, dull tones instead of bright beeps (the spectral center of the
  sounds dropped from roughly 800–1900 Hz to roughly 300–450 Hz).
- **Mic sound volume.** Settings → Voice Typing → Microphone sound now
  has its own volume slider for the mic sounds — for the built-in
  styles and for system notification sounds alike — independent of the
  typing volume.

## 1.60.0 — Nov 19, 2026

- **Enter that follows the app.** The Enter key now does what the field
  expects, Gboard-style: a newline in chats and notes, Send in
  messengers, Search in the browser, Next/Done in forms — with the
  matching icon on the key (return, paper plane, magnifier, arrow,
  checkmark).
- **Dictation cleanup.** A new AI cleanup pass for dictation (Settings
  → Voice Typing → Smart cleanup): filler words, stutters, false starts
  and stray asides are removed, broken sentences are fixed, and spoken
  lists ("one… two… three…") come out as numbered lists. Your voice and
  wording stay yours — and if a cleanup ever drifts too far from what
  you said, the raw transcript is used instead.
- **Voice history in the Clipboard panel.** The Clipboard panel has two
  tabs now: Clipboard and Voice history — every dictation, one tap to
  paste it back. No more digging through Settings.
- **No more jumping.** The whole dictation flow — recording,
  transcribing, back to the keys — runs at one fixed height with fades
  between states. Transcribing keeps the orb on screen while its wave
  settles; nothing pops and nothing resizes.
- **One back arrow, animated panels.** Every panel (emoji, GIF,
  clipboard) returns to the keys with the same back arrow, panels
  crossfade instead of popping, clipboard tabs slide with direction,
  and dictation opens with a short distortion intro on the orb.
- **Mic sounds: redesigned + system sounds.** All mic on/off sounds
  were redesigned, with two new styles (Droplet, Feather). You can also
  switch the mic sounds to your phone's own notification sounds,
  picking one for mic-on and one for mic-off (Settings → Voice Typing →
  Microphone sound → System sounds).

## 1.53.0 — Nov 18, 2026

- **Emoji search, fixed.** The emoji panel now sits above the keys,
  exactly like the GIF panel: tap Search, type, and the results filter
  live in a row over the keyboard. Enter expands them full-height.
- **Update badge on Settings.** The green Update tab in the toolbar is
  gone. When a newer version is ready, a small dark-green UPDATE badge
  appears on the Settings icon instead — and Settings opens with the
  update banner and its Download button right at the top.

## 1.51.0 — Nov 18, 2026

- **Emoji search.** A search field inside the emoji panel, just like
  GIF search — type and the grid filters.
- **Emoji suggestions that actually work.** The suggestion strip now
  uses the official Unicode CLDR keyword database in English, Russian
  and Hebrew (4,000+ emoji): type "piano" or «пианино» and 🎹 is the
  first suggestion, every time.

## 1.50.0 — Nov 18, 2026

- **New launcher icon.** A clean, hand-drawn-style keyboard with a
  microphone — flat and isometric, no glossy AI look.

## 1.49.0 — Nov 18, 2026

- **Enter is Enter.** The Enter key now always inserts a newline. It
  never triggers Send in any app, ever.

## 1.48.0 — Nov 18, 2026

- **Clipboard chip.** Copy anything — a code, an OTP, a snippet — and
  it shows up as a chip in the suggestion strip. One tap pastes it; the
  ✕ dismisses that copy for good. No digging through clipboard history.
- **Dictation keeps the screen awake.** While you dictate, the screen
  no longer falls asleep mid-sentence — and a finished dictation is
  never thrown away if the keyboard closes during transcription.


## 1.47.0 — Nov 17, 2026

- **Version footer.** The Settings home now shows the installed version
  at the bottom.
- **Check for updates.** Setup gets a manual Check for updates button —
  no need to wait for the automatic check.

## 1.46.0 — Nov 17, 2026

In-app updates:

- **Automatic update checks.** The app quietly asks GitHub for the
  latest release every few hours.
- **Green Update tab.** When a newer version is ready, a green Update
  tab with a badge appears in the keyboard toolbar and at the top of
  Settings.
- **Update screen with Download.** Tap the tab to read what's new and
  download the new version from GitHub right in the app.

## 1.45.0 — Nov 17, 2026

- **Get an OpenAI key in one tap.** Settings → Voice Typing links
  straight to OpenAI's API key page — no key yet, no hunting for it.
- **Green microphone status.** "Microphone access: allowed" now shows
  with a green dot and green text when access is granted.

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

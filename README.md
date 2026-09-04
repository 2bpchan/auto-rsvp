# _rvsp_

This is a fork of [Eeman1113/_rvsp_](https://github.com/Eeman1113/_rvsp_), an RSVP (Rapid Serial Visual Presentation) speed reading app.

## What's new since the fork

- **Load text via URL** - populate the reader directly from a link (`#text=...&title=...`), supporting very long content since it's passed in the URL hash rather than a query string
- **Long-word handling** - the focus letter now sits left of center instead of dead center, and long hyphenated words or file paths shrink to fit on screen instead of getting clipped
- **Non-letter word slowdown** - a configurable extra delay (default 50%) *per* character that isn't A-Z, so symbol-heavy words like file paths get progressively more time than a word with just one hyphen (capped at 5 characters, so a long numerical ID doesn't drag on forever)
- **Markdown emphasis rendering** - `*italic*` and `**bold**` markers are stripped and rendered as actual italic/bold styling (including nested `**bold with *italic* inside**`) instead of showing the literal asterisks or counting them toward the slowdown above. The whole word list is resolved up front, so an unmatched marker (no closing partner within the same sentence, capped at 30 words either way) is just left as a literal asterisk rather than getting stuck applying emphasis for the rest of the text
- **Single-word stepping** - previous/next word buttons and `<`/`>` keyboard shortcuts, in addition to the existing 10-word skip
- **Word size setting** - adjustable reader text size (10-200%)
- **Sentence navigation** - the rewind/left-arrow control jumps to the start of the current sentence (press again for the previous sentence); the fast-forward/right-arrow control plays at normal speed until the end of the current sentence, then pauses
- **Enclosing punctuation in the margins** - when the current word is inside parentheses, brackets, braces, or angle brackets, the wrapping characters are stripped from the word and shown large and color-coded (by type) in the left/right margins instead, nested outermost-first, so they don't clutter the word and are easy to notice in peripheral vision. Supports multiple simultaneous/nested levels
- **Sentence-end "poof" effect** - a small [Power Mode](https://github.com/hoovercj/vscode-power-mode/issues/1)-inspired square-poof gif fires near the end of each sentence as it's read during playback, embedded locally so it never depends on an external host. Toggle it off in Settings
- **Delay "wave" for jargon** - words with at least a configurable number of non-letter characters (default 3) get a brightness wave sweeping left to right across the individual letters, timed to traverse the whole word over the first 95% of its display delay and settle back to plain for the last 5% - a visual cue for why the word is lingering

# _rvsp_

This is a fork of [Eeman1113/_rvsp_](https://github.com/Eeman1113/_rvsp_), an RSVP (Rapid Serial Visual Presentation) speed reading app.

## What's new since the fork

- **Load text via URL** - populate the reader directly from a link (`#text=...&title=...`), supporting very long content since it's passed in the URL hash rather than a query string
- **Long-word handling** - the focus letter now sits left of center instead of dead center, and long hyphenated words or file paths shrink to fit on screen instead of getting clipped
- **Non-letter word slowdown** - a configurable extra delay (default 50%) for words containing anything other than A-Z, e.g. hyphenated words or file paths
- **Single-word stepping** - previous/next word buttons and `<`/`>` keyboard shortcuts, in addition to the existing 10-word skip
- **Word size setting** - adjustable reader text size (50-200%)

# FPV Session Timer

Single-page session timer for FPV sim practice. Live at https://weefpv.github.io/session-timer/

## Keyboard controls

| Input | Before start | During warm-up | After warm-up |
|---|---|---|---|
| Space | Start with warm-up | (ignored) | +1 |
| Space ×2 | Start, skip warm-up | (ignored) | Undo last +1 |
| Space ×3 | | End | End |
| P | | Pause / resume | Pause / resume |
| F | Fullscreen | Fullscreen | Fullscreen |

## Touch mode

Settings > Input mode: Auto, Keyboard or Touch. Auto picks Touch when the device's main pointer is a finger.
In Touch mode the tap pad does what Space does, and Pause, Fullscreen and Session info are buttons.
Fullscreen is hidden on iPhone, where Safari doesn't support it for pages.

## Timer

Count up (the default), or count down from 5, 10, 15, 20 minutes or a custom value. Each session type sets a default.
At zero the window flashes, then the display counts overtime as `+m:ss`.

## Settings

Gear icon, top right. Saved per device:

- Warm-up length: 0 to 5 min, default 3
- Hide controls after: 0 to 60 s, default 3 (0 never hides)
- Animation speed: 1 to 100 (5 s to 1 s per rainbow cycle), default 50
- Input mode: Auto, Keyboard or Touch
- Counter label (resets to the session's default when you pick a session)

Reset to defaults restores all of the above.

## Session content

Session descriptions, default counter labels, default timer and warm-up skip are a snapshot of the ClickUp
"01 Session menu" task, in the `SESSIONS` block in `index.html`. The first entry, "Unspecified", is app-only:
it's the default session, with Count up and the "oopsies" label.

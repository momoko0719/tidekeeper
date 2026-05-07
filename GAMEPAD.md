# Ocean Guardian - Gamepad Input Guide

The game uses the browser **Gamepad API**.
**Keyboard and gamepad input both stay enabled** and are merged per player slot.

## Player Slot to Gamepad Index

| Player | Gamepad Index | Notes |
|------|------|------|
| P1 | First detected pad (`0`) | Connect P1 first if possible |
| P2 | `1` | Second connected pad |
| P3 | `2` | Third connected pad |
| P4 | `3` | Fourth connected pad |

Detection order comes from the OS/browser. If players are mismatched, reconnect pads in your intended **P1 -> P4** order.

## Standard Gamepad Mapping

Current config in `index.html`:
- `GP_DEADZONE = 0.22`
- `GP_BTN_ACT = 0` (A / Cross)
- `GP_BTN_GRD = 1` (B / Circle)
- `GP_BTN_ALT = 2` (X / Square)
- `GP_BTN_NEXT = 3` (Y / Triangle)

| Input | In-game behavior |
|------|------|
| **Left Stick (LS)** | Move (radial deadzone applied) |
| **D-Pad** | Move (combined with stick/keyboard, then speed-limited) |
| **Button 0 (A / Cross)** | Primary action: gather seaweed, interact with pond, sell/cook confirm, steal attempt, SSR mash, vote "More", menu continue/start |
| **Button 1 (B / Circle)** | Guard/utility: tap on island to open/cancel build menu, hold on island (>= 0.25s) to activate guard, tap in ocean while holding fish to release, vote "Less" |
| **Button 2 (X / Square)** | Vote "Same" during verdict screen |
| **Button 3 (Y / Triangle)** | "Next Round" confirm after all votes are submitted |

Action buttons are edge-triggered (press transition), which prevents auto-repeat from long holds.

## Guard and Build Timing Rules

- **Island tap B** (`< 0.25s`): open build/upgrade menu.
- **Island hold B** (`>= 0.25s`): enable guard mode.
- Releasing B after a long hold disables guard and starts cooldown.
- Guard can also expire automatically (then cooldown starts).
- If guard cooldown is active, pressing B on island shows cooldown feedback.

## SSR Fish Clash

During SSR clash, only the two involved players can score by mashing **A (Button 0)**.
If A was already held before entering clash, players must release and press again to register new taps.

## Keyboard Reference (Unchanged)

| Player | Move | Act | Grd |
|------|------|-----|-----|
| P1 | WASD | E | Q |
| P2 | Arrow keys | / | . |
| P3 | T F G H | Y | R |
| P4 | I J K L | O | U |

## Browser and Debug Notes

- Use a modern browser (Chrome, Edge, Firefox).
- Click the game once so the page has focus before using a controller.
- If your physical pad layout differs, update button mapping constants in `index.html` (`GP_BTN_ACT`, `GP_BTN_GRD`, `GP_BTN_ALT`, `GP_BTN_NEXT`) and deadzone (`GP_DEADZONE`).

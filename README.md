# Dorn's Optimal Tool Use

For **S.T.A.L.K.E.R. G.A.M.M.A.** — when disassembling items, wears the lowest-condition tool stack that will still survive the operation, so your good tools stay available for crafting and repair.

## What this mod does

GAMMA's **Disassembly Item Tweaks** already picks the right tool *type* per item (grooming kit → swiss knife → multitool/leatherman, with outfits preferring knife types). This mod does **not** change that priority.

It only fixes *which stack* gets worn down:

- **Keypress / context-menu disassembly** — after DIT picks the tool type, selects the lowest-condition instance of that type that won't break (matching DIT's break thresholds when configured)
- **Drag-and-drop** — you still drag any valid tool, but degradation is redirected to the lowest stack of that same type (not the top-of-stack good one MO2 shows)
- **Autolooter / other callers** of `get_suitable_dtool` — same stack fix, without overriding type selection

## GAMMA tools

- `grooming` — grooming kit (lowest tier, used first when applicable)
- `swiss_knife` — swiss army knife
- `leatherman_tool` — multitool (weapons; fallback for other items)

## Installation

1. Download the latest release (when published) or install the folder via MO2
2. Load **after** Disassembly Item Tweaks (script is named `zzzz_` for late load order)
3. Enable in Mod Organizer 2 like any other mod

## Options (MCM)

- **Enabled** — toggle the fix on/off (default: on)
- **Debug log** — log which stack was selected or redirected

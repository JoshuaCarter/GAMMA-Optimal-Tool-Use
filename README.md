# Dorn's Optimal Tool Use

For **S.T.A.L.K.E.R. G.A.M.M.A.** — when disassembling items, automatically uses the lowest-condition tool that will still survive the operation, so your good tools stay available for crafting and repair.

## What this mod does

- Replaces vanilla disassembly auto-tool selection (`item_parts.get_suitable_dtool`)
- Scans your inventory for every valid tool of the relevant type (Leatherman for weapons, any disassembly tool for other items)
- Picks the lowest-condition instance whose condition is still above the degradation cost for that use
- Drag-and-drop still accepts whatever tool you drop, but degradation is redirected to the lowest-condition stack of that same tool type (so the top-of-stack good one is not worn down)

## Installation

1. Download the latest release (when published) or install the folder via MO2
2. Enable in Mod Organizer 2 like any other mod

## Options (MCM)

- **Enabled** — toggle the fix on/off (default: on)
- **Debug log** — log which tool was auto-selected

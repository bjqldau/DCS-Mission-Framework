# Scripting Guide

## Purpose

Use scripting only when it improves mission reliability, replayability or player experience beyond what can be achieved cleanly with Mission Editor triggers.

## Folder roles

```text
scripts/custom/   Project-specific Lua
scripts/mist/     MIST library and integration notes
scripts/moose/    MOOSE library and integration notes
```

Do not commit multiple unexplained versions of the same framework. Record the version used and any local modifications.

## General rules

- Prefer the simplest workable solution.
- Keep script files focused on one responsibility.
- Use descriptive function, variable and flag names.
- Avoid global variables where practical.
- Validate groups and zones before acting on them.
- Log useful errors without flooding `dcs.log`.
- Ensure optional enhancements fail gracefully.
- Document required Mission Editor triggers and load order.

## Recommended load order

A typical scripted mission may load:

1. External framework library, if required.
2. Shared utility functions.
3. Mission initialisation.
4. Feature modules such as radio menus, spawning or scoring.
5. Mission-specific event logic.

Use clearly named `MISSION START` triggers and short delays only where DCS initialisation requires them.

## File headers

Each custom script should begin with:

```lua
-- Script: carrier-support.lua
-- Mission: reusable / mission name
-- Purpose: short description
-- Dependencies: none / MIST version / MOOSE version
-- Load order: after framework.lua
-- Updated: YYYY-MM-DD
```

## Debugging

- Use a documented debug flag or configuration variable.
- Keep debug messages distinct from player-facing messages.
- Remove or disable noisy debug output before release.
- Record relevant errors from `Saved Games/DCS/Logs/dcs.log` when investigating failures.

## Multiplayer considerations

- Test scripts on a multiplayer host.
- Confirm F10 menu commands work for clients and intended coalitions/groups.
- Avoid logic that assumes the host occupies a player slot.
- Consider late activation, late joining and destroyed groups.
- Do not assume event order will be identical in every run.

## Framework selection

### Mission Editor triggers

Use for straightforward activation, messages, flags and objective checks.

### MIST

Use where lightweight helper functions or dynamic group operations are needed.

### MOOSE

Use where its object model and higher-level systems provide a clear benefit, such as complex dispatching or reusable operational behaviours.

### Custom Lua

Use for small, project-specific logic that does not justify a larger framework.

The presence of a framework is not a quality measure. Reliability and maintainability are the goals.

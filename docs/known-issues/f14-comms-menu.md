# F-14 Communications Menu Mouse Bug

## Summary

When flying the Heatblur F-14 with Easy Communications enabled, the Communications/F10 menu may open normally but ignore mouse clicks.

## Test environment

- DCS Open Beta 2.9.28.26385
- Heatblur F-14B
- Supercarrier hot start on catapult
- Mission with Easy Communications forced ON

## Reproduction

1. Spawn in the F-14.
2. Open the Communications menu.
3. Observe that menu items cannot be selected with the mouse.

## Comparison

Using the same mission and settings, the F/A-18C communications menu remains fully mouse clickable.

## Workaround

1. Bind the F-14 "Tomcat Ball" command.
2. After spawning, press the Tomcat Ball binding once.
3. Reopen the Communications menu.
4. Mouse interaction is restored.

## Status

Observed and reproduced by the Super Sonic group. The evidence currently suggests an F-14-specific interaction with Easy Communications rather than a mission framework issue. This behaviour should be revalidated after future DCS or Heatblur updates.
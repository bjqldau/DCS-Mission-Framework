# Super Sonic Troubleshooting

This guide captures repeatable problems found during mission building and squadron testing. Use the baseline settings guide first, then work through the relevant section below.

## F-14 communications menu opens but mouse clicks do not work

### Symptoms

- The communications or F10 menu opens.
- Mouse clicks do not select menu items.
- Joystick or keyboard command-menu controls may still work.

### Likely cause

**Easy Communication** is enabled or forced by the mission.

This fault was reproduced by forcing Easy Communication on in Mission Options, starting an F-14 on Supercarrier Catapult 1, and opening the comms menu from a joystick binding.

### Fix

1. Open **Options > Gameplay**.
2. Turn **Easy Communication** off.
3. Turn **No force from mission, use mine** off.
4. In Mission Editor, ensure **Easy Communication** is not enforced on.
5. Fully restart DCS.
6. Reload the mission and test the menu before using any workaround.

### Immediate workaround

Press the bound **Tomcat Ball** command. After the voice call, mouse interaction with the menu may begin working immediately.

The workaround appears to reset or initialise the F-14 menu/input state, but Easy Communication should still remain off for normal squadron use.

### Investigation record

See GitHub Issue #6 for the original observations and controlled tests.

## SRS shows not connected

1. Confirm the mission is running in multiplayer or on the intended server.
2. Confirm DCS-SRS is running.
3. Check the configured server address and auto-connect settings.
4. Confirm Windows is using the intended microphone and headset.
5. Verify the SRS overlay and push-to-talk bindings.
6. Restart SRS, then DCS, if the connection state remains stale.

The red **SRS not connected** message can be expected while testing a mission locally without joining an SRS-enabled server.

## Carrier TACAN or ICLS not received

1. Confirm the carrier group's TACAN and ICLS settings in Mission Editor.
2. Confirm the published channel and callsign match the briefing and kneeboard.
3. Confirm the aircraft equipment is set to the correct band and channel.
4. Check that the carrier task or activation logic has not been removed or delayed.
5. Test from a known-good hot-start aircraft before changing mission logic.

## F10 menu item missing

1. Confirm the player is in the correct coalition and aircraft group.
2. Check whether the menu item is created for coalition, group or all players.
3. Confirm the required trigger or script has run.
4. Check DCS log output for script errors.
5. Test in multiplayer as well as single player, because group IDs and player slots can behave differently.

## Spawn slot unavailable or blocked

1. Confirm the aircraft start type and carrier parking/catapult assignment.
2. Check for overlapping static objects or deck aircraft.
3. Confirm another client is not occupying the same slot.
4. Reduce deck congestion and retest.
5. Validate all intended player slots during the multiplayer acceptance test.

## Reporting a new problem

When creating a GitHub issue, include:

- DCS version
- Mission file and version
- Aircraft and seat
- Single-player or multiplayer
- Exact start location or slot
- Relevant gameplay and mission-option settings
- Steps to reproduce
- Expected result
- Actual result
- Workarounds tested
- Screenshots, short video or logs where useful

A finding should only be promoted into this guide once it is repeatable or has a reliable workaround.

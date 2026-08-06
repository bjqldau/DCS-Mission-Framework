# Super Sonic Baseline DCS Settings

This page records the recommended baseline DCS configuration for Super Sonic missions. It focuses on settings that can affect mission behaviour, multiplayer compatibility, radios and carrier operations.

These are baseline settings rather than mandatory cosmetic preferences. Individual pilots may adjust graphics, controls, views and accessibility options provided they do not interfere with mission functionality.

## Gameplay settings

Open **Options > Gameplay** and use the following baseline:

| Setting | Recommended value | Notes |
|---|---:|---|
| Easy Communication | **Off** | Important for reliable F-14 comms-menu behaviour. See the known issue below. |
| Radio Assists | **Off** | Prevents automatic radio assistance from masking radio setup problems. |
| No force from mission, use mine | **Off** | Allows mission-enforced gameplay settings to apply as intended. |
| F10 Map User Marks | **On** | Required where mission scripts or players use map marks. |
| Units | **Imperial** | Matches the normal F-14 and carrier workflow. |
| G-Effects | **Simulation** | Recommended squadron baseline. |
| Wake Turbulence | Optional | May be enabled where performance permits. |
| Labels | Squadron preference | Mission-specific guidance may override this. |

After changing gameplay settings, fully exit and restart DCS before testing a suspected configuration problem.

## Mission options

Mission designers should avoid forcing **Easy Communication** on.

Where consistent gameplay settings are important, use the Mission Editor's **Mission Options** panel and document any enforced values in the mission briefing or release notes.

Pilots should leave **No force from mission, use mine** unchecked so those mission settings can take effect.

## F-14 control bindings

Before joining a mission, confirm that the following commands are bound and tested:

- Communications menu
- Tomcat Ball
- SRS push-to-talk controls
- Aircraft radio push-to-talk controls used by the crew
- Jester menu controls where applicable

The **Tomcat Ball** command is particularly important because it provides a workaround for the Easy Communication comms-menu issue described below.

## SRS baseline

Before mission night:

1. Confirm DCS-SRS is installed and current.
2. Confirm the SRS overlay reports a connection to the mission server.
3. Test the required push-to-talk bindings.
4. Confirm the correct radio is selected and transmitting.
5. Check microphone level and audio devices before entering the aircraft.

## Known issue: F-14 comms menu cannot be clicked

### Symptoms

- The communications or F10 menu opens normally.
- Menu items cannot be selected with the mouse.
- Joystick or keyboard command-menu navigation may still work.

### Confirmed trigger

During testing in the F-14 on a Supercarrier catapult, forcing **Easy Communication** on reproduced the fault.

### Preferred fix

1. Set **Easy Communication** to **Off** in **Options > Gameplay**.
2. Ensure the mission does not force Easy Communication on.
3. Leave **No force from mission, use mine** unchecked.
4. Restart DCS and reload the mission.

### Workaround

Press the bound **Tomcat Ball** command. The voice call is heard and mouse interaction with the menu may immediately begin working again.

This workaround appears to reinitialise the F-14 command-menu or input state. It should not replace the preferred baseline setting of Easy Communication off.

## First-time validation

A new player should complete the following test before joining a full squadron mission:

- Enter an F-14 hot start on the carrier.
- Open the communications menu using the normal control binding.
- Confirm menu items can be selected with the mouse.
- Confirm the Tomcat Ball command is bound and produces the expected voice call.
- Confirm SRS connects and push-to-talk works.
- Confirm F10 map marks can be created and viewed.

Record new repeatable configuration problems in the repository issue tracker and add confirmed fixes to the troubleshooting guide.

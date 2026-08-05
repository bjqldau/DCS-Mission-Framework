# Mission Build Checklist

Use this checklist before moving a mission from `missions/development/` to `missions/released/`.

## File and version control

- [ ] Mission was created from a copy of the correct base template.
- [ ] File name follows the naming convention.
- [ ] Mission version or revision is recorded in the briefing or release notes.
- [ ] No unintended backup, temporary or extracted files are included.
- [ ] Changes are committed with a meaningful Git message.

## Scenario and briefing

- [ ] Mission objective and operational context are clear.
- [ ] Player tasking, route, target and restrictions are stated.
- [ ] Success, partial success and failure conditions are understandable.
- [ ] Expected duration is stated or apparent.
- [ ] Required modules, maps and asset packs are identified.
- [ ] Briefing images are legible at normal DCS briefing size.
- [ ] Bullseye, reference points and named areas match the Mission Editor.

## Player aircraft

- [ ] Correct aircraft variants and liveries are used.
- [ ] Player and client slots are correct.
- [ ] Hot, cold, runway or airborne starts are intentional.
- [ ] Fuel and stores support the planned task.
- [ ] Countermeasures and gun ammunition are appropriate.
- [ ] Waypoints and target points are correct.
- [ ] Radio presets are verified where the module supports them.
- [ ] TACAN and ICLS information matches the briefing and kneeboard.

## Carrier operations

- [ ] Carrier course and speed are intentional.
- [ ] Wind-over-deck is suitable for launch and recovery.
- [ ] Player aircraft spawn correctly on the carrier.
- [ ] Catapult launches have been tested.
- [ ] Carrier TACAN works and has the correct identifier.
- [ ] ICLS works on the briefed channel.
- [ ] Recovery lighting and time of day are suitable.
- [ ] Marshal and recovery frequencies are correct.
- [ ] Rescue helicopter behaviour is acceptable.
- [ ] Recovery tanker is available when required.

## Support aircraft

- [ ] AWACS route, altitude, callsign and frequency are correct.
- [ ] Tanker track, altitude, speed, TACAN and frequency are correct.
- [ ] Support aircraft have sufficient fuel and sensible reaction-to-threat settings.
- [ ] Support aircraft do not interfere with carrier launch or recovery.
- [ ] Escort or replacement logic is tested if used.

## AI and threats

- [ ] AI routes and tasking work from mission start.
- [ ] Triggered AI activates at the intended time or condition.
- [ ] AI skill levels are deliberate.
- [ ] Air defences use suitable alarm state and engagement rules.
- [ ] Enemy forces do not detect or engage players unrealistically early without design intent.
- [ ] Mission remains playable if an AI group behaves imperfectly.

## Triggers and scripting

- [ ] Trigger names are descriptive and grouped logically.
- [ ] Flags and conditions do not conflict.
- [ ] Primary objective logic has been tested.
- [ ] Mission success and failure messages appear correctly.
- [ ] F10 radio menu items appear and can be selected.
- [ ] Script files load in the correct order.
- [ ] Missing or failed scripts degrade gracefully where practical.
- [ ] Debug messages and test triggers have been removed or disabled.

## Weather and environment

- [ ] Mission date and time suit the intended lighting.
- [ ] Sun position does not unnecessarily obscure the target, formation or carrier approach.
- [ ] Wind directions and speeds are checked at all configured layers.
- [ ] Clouds, visibility, fog, turbulence and precipitation are intentional.
- [ ] Sea conditions are acceptable for the desired carrier experience.

## Multiplayer test

- [ ] Mission loads on the host without errors.
- [ ] All intended players can occupy slots.
- [ ] Late joining has been tested if supported.
- [ ] Radio menu works for clients, not only the host.
- [ ] Triggers fire correctly in multiplayer.
- [ ] Performance is acceptable during the busiest phase.
- [ ] At least one full launch-to-recovery play-through has been completed.

## Release

- [ ] Known issues are documented.
- [ ] Final `.miz` is copied to `missions/released/`.
- [ ] Release notes summarize meaningful changes.
- [ ] The release commit or tag is identifiable.

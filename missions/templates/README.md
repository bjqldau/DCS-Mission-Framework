# Mission Templates

Store tested, reusable map templates here. Do not build a scenario directly in the stable template file.

## Expected template contents

- Player aircraft slots.
- Carrier group and navigation aids where applicable.
- Rescue helicopter.
- Tanker and AWACS support.
- Tested weather and lighting.
- Standard radio plan.
- Common briefing and kneeboard placeholders.
- Required shared script initialisation.

## Workflow

1. Copy the required template into `missions/development/`.
2. Rename the copy using the mission naming convention.
3. Add scenario-specific forces, triggers, assets and briefing material to the copy.
4. Update a template only when improving reusable framework behaviour.
5. Re-test launch, radios, support assets and recovery after every template change.

## Template status

The first planned template is Syria. Its initial release should not be labelled `v1.0` until carrier operations, support aircraft, radio settings, weather and multiplayer behaviour have been verified.

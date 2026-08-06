# Development Mission Roadmap

This page tracks planned work and items that are not yet verified. Move completed, player-visible changes into the changelog and preserve important findings in the development log.

## In progress

- Test the `MIGS` trigger in single-player and multiplayer.
- Confirm the opposing aircraft group activates only once.
- Confirm the trigger responds to any BLUE coalition unit rather than a specific player group.
- Verify the activated group follows its intended route and tasking.
- Confirm forced Easy Communication behaves consistently for all squadron players.

## Next

- Validate carrier TACAN, ICLS and radio services from a fresh player profile.
- Confirm F-14 radio presets and Prepare Mission settings survive mission distribution.
- Run a complete three-player launch, mission and carrier-recovery test.
- Update the mission briefing and kneeboard with any required player procedures.
- Decide the first development version number and rename the `.miz` file accordingly.

## Before release

- Complete the mission build checklist.
- Test all triggers from a clean mission start.
- Test player death, respawn and slot changes where applicable.
- Confirm no development-only messages or test triggers remain.
- Synchronise the `.miz` file, briefing, kneeboard and documentation.
- Move the tested mission to the appropriate release folder and create a Git tag.

## Parking lot

Ideas that are useful but not currently committed to the next release:

- Additional aircraft slots.
- More dynamic opposing-aircraft behaviour.
- Tanker and AWACS automation improvements.
- Automated kneeboard generation.
- Mission completion and debrief logic.

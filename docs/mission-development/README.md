# Mission Development Records

This folder records changes made to missions while they are under development.

Use these files for different purposes:

- [CHANGELOG.md](CHANGELOG.md) — concise record of what changed in each development version.
- [development-log.md](development-log.md) — engineering notes explaining why a change was made, what was tested and what was learned.
- [roadmap.md](roadmap.md) — planned work, open decisions and items awaiting testing.

## What belongs where

### Changelog

Record player-visible or mission-behaviour changes, for example:

- Easy Communication forced on.
- MiG group activates when a BLUE unit enters a trigger zone.
- Tanker frequency changed.
- Carrier recovery conditions adjusted.

### Development log

Record investigation and design reasoning, for example:

- Why Easy Communication remains enabled.
- Test results comparing the F-14 and F/A-18C.
- Why a trigger uses coalition entry rather than a specific aircraft group.
- Failed approaches that should not be repeated.

### Roadmap

Record work that is planned but not yet complete or verified.

## Recommended mission-editing workflow

1. Make one logical change in the Mission Editor.
2. Save the development `.miz` file.
3. Add a short line to the changelog.
4. Add detail to the development log only when the reasoning or test result will matter later.
5. Test the changed behaviour.
6. Mark the result in the development log or roadmap.
7. Commit the `.miz` file and its documentation together with a clear commit message.

Example commit messages:

- `Force Easy Communication for squadron missions`
- `Trigger MiG intercept on BLUE zone entry`
- `Document F-14 comms menu workaround`

## Versioning note

During development, use a clear filename or release label such as `v0.1.1-dev`. Stable, tested versions can be promoted to `missions/templates/` or `missions/released/` and tagged in Git.
# Development Mission Changelog

This changelog records changes made to the current development mission. Keep entries concise and describe observable mission behaviour rather than every Mission Editor click.

## Unreleased — 2026-08-06

### Added

- Forced **Easy Communication ON** in Mission Options to retain automatic radio-frequency tuning for squadron players.
- Added trigger logic for the opposing aircraft group using the `MIGS` trigger zone.
- The opposing aircraft group now activates when **any BLUE coalition unit** enters the `MIGS` zone.

### Changed

- Adopted the F-14 **Tomcat Ball** command as the squadron workaround for the communications-menu mouse issue when Easy Communication is enabled.

### Testing

- Confirmed the F/A-18C communications menu remains mouse-interactive with Easy Communication enabled.
- Confirmed the F-14 communications menu is initially not mouse-interactive with Easy Communication enabled.
- Confirmed pressing **Tomcat Ball** once restores F-14 mouse interaction with the communications menu.
- Zone-triggered aircraft activation still requires verification of one-time activation, coalition filtering and expected mission behaviour.

---

## Entry template

```markdown
## v0.x.x-dev — YYYY-MM-DD

### Added
- 

### Changed
- 

### Fixed
- 

### Testing
- 
```

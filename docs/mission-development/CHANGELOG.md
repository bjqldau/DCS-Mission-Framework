# Development Mission Changelog

This changelog records changes made to the current development mission. Keep entries concise and describe observable mission behaviour rather than every Mission Editor click.

## v0.1.8 — Validated baseline — 2026-09-27

### Changed

- Sanitised the Syria base template by removing mission-specific enemy units and associated scenario triggers.
- Retained reusable carrier-group, support-aircraft, navigation, communications and landing-practice infrastructure.
- Carrier remains preset for **TACAN 74X / ICLS 11**; Texaco uses **11Y**.
- **Easy Communication ON** remains a deliberate squadron accessibility setting.
- **Wake Turbulence OFF** remains the baseline setting.

### Testing

- Multiplayer flight-tested with two F-14B(U) clients.
- Both players successfully launched, completed a basic sortie and recovered aboard USS Theodore Roosevelt.
- Treat **SSO Base Template - Syria v0.1.8.miz** as the known-good sanitised baseline for new missions.

---

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

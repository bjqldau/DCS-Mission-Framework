# DCS Mission Framework

Reusable mission templates, documentation, assets and scripts for the **Super Sonic** DCS flying group

## Purpose

This repository makes DCS mission creation more consistent, repeatable and maintainable. The initial focus is carrier-based F-14 operations for two or three players, with enough realism to create immersion without sacrificing enjoyment.

## Project status

**Framework setup:** in progress  
**First base template:** Syria  
**Current milestone:** document and validate the reusable carrier environment

The repository currently contains the initial project structure and design standards. The next major addition will be the working Syria base-template `.miz` file.

## Start here

Read the [Super Sonic Mission Bible](docs/mission-bible.md) for the overall design philosophy and workflow.

### Players

New and returning players should review:

- [Baseline DCS settings](docs/baseline-dcs-settings.md)
- [New player checklist](docs/new-player-checklist.md)
- [Troubleshooting](docs/troubleshooting.md)

The baseline settings guide records configuration choices that can affect mission behaviour, including the F-14 communications-menu problem caused by Easy Communication.

### Mission designers

Core references:

- [Mission standards](docs/mission-standards.md)
- [Mission build checklist](docs/mission-build-checklist.md)
- [Carrier standards](docs/carrier-standards.md)
- [Radio plan](docs/radio-plan.md)
- [Weather standards](docs/weather-standards.md)
- [Naming conventions](docs/naming-conventions.md)
- [Scripting guide](docs/scripting-guide.md)

## Repository structure

```text
missions/
  templates/      Tested Mission Editor base templates
  development/    Missions currently being built or tested
  released/       Tested mission releases

docs/             Mission Bible, standards, player setup and checklists

assets/
  briefings/      Briefing source material and exported images
  kneeboards/     Mission and aircraft kneeboard pages
  audio/          Radio messages, voiceovers and sound effects
  images/         Logos, maps, references and thumbnails

scripts/
  custom/         Project-specific Lua scripts
  mist/           MIST library or integration notes
  moose/          MOOSE library or integration notes
```

## Mission philosophy

- Designed primarily for the Super Sonic group.
- Usually two or three human pilots.
- Carrier-based F-14 operations are the default starting point.
- Typical session duration is approximately two to three hours.
- Hot starts are preferred unless startup is part of the mission experience.
- Procedures should feel credible, but fun and reliability take priority over strict simulation.
- Base templates handle repetitive setup such as the carrier group, rescue helicopter, tanker, AWACS, weather, navigation aids and common radio services.

## Basic workflow

1. Copy the appropriate `.miz` file from `missions/templates/` into `missions/development/`.
2. Rename it using the project naming convention.
3. Build the scenario without modifying the stable template.
4. Test in small increments and keep the briefing synchronized with the mission.
5. Complete the mission build checklist.
6. Test multiplayer startup, objectives, radio menu, carrier recovery and completion logic.
7. Move the tested version to `missions/released/` and create an identifiable release commit or tag.

## Initial roadmap

1. Import the Syria base template.
2. Record and verify carrier TACAN, ICLS and radio services.
3. Confirm tanker, AWACS and rescue-helicopter behaviour.
4. Finalise the standard weather and lighting preset.
5. Conduct a multiplayer three-player launch and recovery test.
6. Release the Syria template as `v1.0`.
7. Build the first scenario from the released template.

## Guiding rule

The `.miz` file defines what DCS is actually configured to do. The documentation defines what the framework intends to do. The briefing and kneeboard must agree with the tested mission file.

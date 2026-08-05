# DCS Mission Framework

Reusable mission templates, documentation, assets, and scripts for the **Super Sonic** DCS flying group.

## Purpose

This repository is intended to make DCS mission creation consistent, repeatable, and easier to maintain. The initial focus is carrier-based F-14 operations for two to three players, with enough realism to create immersion without sacrificing enjoyment.

## Repository structure

```text
missions/
  templates/      Reusable Mission Editor base templates
  development/    Missions currently being built or tested
  released/       Tested mission releases

docs/
  mission-standards.md
  mission-build-checklist.md
  carrier-standards.md
  radio-plan.md
  weather-standards.md
  naming-conventions.md

assets/
  briefings/      Briefing source material and exported images
  kneeboards/     Mission and aircraft kneeboard pages
  audio/          Radio messages, voiceovers, and sound effects
  images/         Logos, maps, reference images, and thumbnails

scripts/
  custom/         Project-specific Lua scripts
  mist/           MIST library or integration notes
  moose/          MOOSE library or integration notes
```

## Mission philosophy

- Designed primarily for the Super Sonic group.
- Usually two or three human pilots.
- Carrier-based F-14 operations are the default starting point.
- Typical mission duration: approximately two to three hours.
- Procedures should feel credible, but fun and reliability take priority over strict simulation.
- Base templates should handle repetitive setup: carrier group, rescue helicopter, tanker, AWACS, weather, navigation aids, and common radio frequencies.

## Basic workflow

1. Copy the appropriate `.miz` file from `missions/templates/` into `missions/development/`.
2. Rename it using the project naming convention.
3. Build the scenario without modifying the original template.
4. Complete the mission build checklist.
5. Test multiplayer startup, objectives, radio menu, carrier recovery, and mission completion logic.
6. Move the tested version to `missions/released/` and tag the release if appropriate.

## Current status

Initial project framework created. The next major repository addition should be the first working Syria base template.

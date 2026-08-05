# Super Sonic Mission Bible

## Purpose

The Mission Bible is the top-level design reference for the Super Sonic DCS mission framework. It explains how the supporting standards fit together and provides a stable baseline for future templates and missions.

## Mission identity

Super Sonic missions are designed for a small group of friends who value credible aviation, teamwork and carrier operations without turning a weekly flight into an administrative exercise.

The normal experience is:

- Two or three human pilots.
- Carrier-based F-14 operations.
- Hot-start aircraft unless startup is a deliberate mission feature.
- A two-to-three-hour session including launch and recovery.
- Semi-realistic procedures with reliability and enjoyment taking priority.

## Framework hierarchy

1. **Mission Bible** — overall philosophy and workflow.
2. **Base templates** — tested map-specific foundations.
3. **Mission standards** — common design rules.
4. **Specialist standards** — carrier, radio, weather and naming guidance.
5. **Development missions** — active scenario builds.
6. **Released missions** — tested versions suitable for group use.

## Source-of-truth rules

- The `.miz` file is the source of truth for actual Mission Editor configuration.
- The documentation is the source of truth for intended standards and workflow.
- The briefing and kneeboard must agree with the final `.miz` file.
- When DCS behaviour differs from the documentation, record the tested behaviour and update the standard.

## Base-template policy

A base template should contain only reusable components, such as:

- Carrier group and navigation aids.
- Rescue helicopter.
- Recovery tanker.
- AWACS.
- Common weather and lighting.
- Standard player slots.
- Common radio plan.
- Reusable trigger or script initialisation.

Scenario-specific targets, enemy forces and story events should normally be added only to a development copy.

## Build workflow

1. Select the correct map template.
2. Copy it into `missions/development/`.
3. Rename it using the naming standard.
4. Write the mission concept and player objective before adding extensive units.
5. Build and test in small increments.
6. Keep radio, navigation and briefing information synchronised.
7. Complete a multiplayer launch-to-recovery test.
8. Complete the mission build checklist.
9. Move the approved `.miz` into `missions/released/`.
10. Commit with clear release notes.

## Design priorities

In order of importance:

1. Mission loads and works reliably.
2. Players understand their task.
3. Launch, navigation, combat and recovery form a coherent experience.
4. Tactical decisions matter.
5. The scenario feels credible.
6. Additional scripting, audio and visual polish enhance the experience.

## Change control

- Do not overwrite a stable base template during mission development.
- Use Git commits as meaningful save points.
- Use a branch or pull request for substantial framework changes.
- Record why a standard changed, especially when driven by a DCS update or module limitation.
- Keep released missions unchanged where possible; publish a new version instead.

## Supporting documents

- [Mission standards](mission-standards.md)
- [Mission build checklist](mission-build-checklist.md)
- [Carrier standards](carrier-standards.md)
- [Radio plan](radio-plan.md)
- [Weather standards](weather-standards.md)
- [Naming conventions](naming-conventions.md)
- [Scripting guide](scripting-guide.md)

## Immediate roadmap

1. Import and review the Syria base template.
2. Record the actual carrier, tanker, AWACS, TACAN, ICLS and radio settings.
3. Validate weather and lighting from the F-14 cockpit.
4. Complete a three-player carrier launch and recovery test.
5. Promote the tested Syria template to version `v1.0`.
6. Build the first mission from that template.

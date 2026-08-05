# Carrier Standards

## Purpose

This document defines the default carrier configuration for Super Sonic missions. Exact channels, frequencies and operating conditions must be verified in each `.miz` file and copied into the briefing and kneeboard.

## Default operating concept

- Carrier-based F-14 operations are the normal baseline.
- Missions will usually use hot starts on the carrier.
- The carrier group should support launch, mission execution and recovery without excessive repositioning.
- Carrier course, speed and ambient wind must be considered together to produce useful wind over deck.
- Recovery geometry and lighting should be tested from the actual player cockpit.

## Carrier group

- Use clear group and unit names, including the carrier name and role.
- Set a deliberate course and speed rather than leaving defaults.
- Keep escorts far enough from the landing pattern and tanker track to avoid interference.
- Ensure escort formations remain stable during turns.
- Confirm the carrier does not reach a waypoint or begin an unexpected turn during the planned recovery window.

## Navigation aids

For every mission, record and verify:

| Item | Required entry |
|---|---|
| Carrier TACAN | Channel, X/Y mode and identifier |
| ICLS | Channel |
| Carrier callsign | Mission Editor value |
| Marshal frequency | Frequency and modulation |
| Tower frequency | Frequency and modulation |
| Departure frequency | Frequency and modulation, if separate |

Do not rely on remembered values. The briefing, kneeboard and Mission Editor must agree.

## Launch

- Verify every client slot spawns in a usable location.
- Test simultaneous or closely sequenced launches for the expected number of players.
- Confirm deck equipment and AI aircraft do not block player taxi routes.
- Avoid scripted carrier turns during launch.
- For hot starts, verify that required navigation and radio equipment can be configured without using Prepare Mission unless that workflow is intentionally supported.

## Recovery

- Define the intended recovery case in the briefing when relevant.
- Ensure the carrier remains on a stable recovery course for the expected window.
- Test the approach at the mission time and weather settings.
- Check that the sun is not positioned directly in the pilot's primary scan or approach view unless deliberately intended.
- Confirm deck lighting and visibility are appropriate.
- Test bolter and wave-off recovery options.

## Recovery tanker

- Use a tanker when mission distance, fuel state or recovery complexity justifies it.
- The tanker track should be close enough to support recovery without conflicting with the landing pattern.
- Record tanker callsign, frequency, TACAN, altitude and speed.
- Verify the tanker remains available for the expected recovery window.

## Rescue helicopter

- Position and task the rescue helicopter so it follows the carrier reliably.
- Ensure it does not obstruct the deck, landing pattern or player taxi routes.
- Treat rescue-helicopter behaviour as immersion support; the mission should not depend on perfect AI execution.

## Template validation

Before promoting a carrier setup into a base template:

- [ ] Launch all intended player slots.
- [ ] Verify TACAN and ICLS from the cockpit.
- [ ] Confirm radio menu access with the selected communications settings.
- [ ] Fly at least one complete recovery.
- [ ] Confirm the carrier remains on the intended course throughout the recovery window.
- [ ] Confirm tanker, AWACS and rescue helicopter remain functional.

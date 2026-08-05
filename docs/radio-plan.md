# Radio Plan

## Purpose

This file defines how radio information should be organised. It deliberately avoids hard-coding channels and frequencies until they are confirmed in the base template.

## Principles

- Use the same role-to-frequency pattern across missions where practical.
- Keep essential player communications simple.
- Avoid assigning the same frequency to unrelated services unless intentionally simulating a shared net.
- Verify frequency, modulation and callsign in the Mission Editor.
- Copy the final values into the briefing and kneeboard.
- Where module preset support is limited, clearly identify which frequencies require manual tuning.

## Standard roles

| Role | Callsign | Frequency | Modulation | TACAN/ICLS | Notes |
|---|---|---:|---|---|---|
| Player/package common | TBD | TBD | TBD | — | Primary human coordination net |
| Carrier marshal | TBD | TBD | TBD | — | Arrival and marshal |
| Carrier tower | TBD | TBD | TBD | — | Launch and recovery |
| AWACS | TBD | TBD | TBD | — | Picture and control |
| Recovery tanker | TBD | TBD | TBD | TBD | Callsign, TACAN and refuelling frequency |
| Mission tanker | TBD | TBD | TBD | TBD | Separate from recovery tanker if used |
| Strike/control | TBD | TBD | TBD | — | JTAC, FAC(A), command or package control |
| Guard/emergency | Standard | As applicable | AM | — | Monitor where supported |

## Aircraft preset guidance

For each flyable type, record:

- Radio equipment available to the pilot and crew.
- Preset channel number and assigned frequency.
- Whether the preset can be configured in the Mission Editor.
- Whether Prepare Mission is required or reliable for that module.
- Any hot-start limitations.

### F-14 notes

The F-14 radio setup varies by variant and module implementation. Do not assume that a preset, TACAN or ICLS value has been loaded until verified from the cockpit in the current DCS release.

## Mission-specific radio card

Each mission should include a compact table like this:

| Channel/service | Frequency | Modulation | Callsign | Remarks |
|---|---:|---|---|---|
| Package |  |  |  |  |
| Carrier marshal |  |  |  |  |
| Carrier tower |  |  |  |  |
| AWACS |  |  |  |  |
| Tanker |  |  |  | TACAN:  |
| Other |  |  |  |  |

## Validation

- [ ] Frequencies do not conflict unintentionally.
- [ ] Modulation is correct.
- [ ] Callsigns match the Mission Editor.
- [ ] Player presets are checked from the cockpit.
- [ ] F10 radio menu works with the selected communications settings.
- [ ] Briefing and kneeboard match the mission file.

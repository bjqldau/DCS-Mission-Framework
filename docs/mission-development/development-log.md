# Mission Development Log

This is the engineering notebook for the current development mission. Use it to preserve decisions, test evidence and lessons that would be difficult to reconstruct from the `.miz` file alone.

## 2026-08-06 — Easy Communication and F-14 menu behaviour

### Problem

With Easy Communication enabled, the F-14 communications menu opened but did not accept mouse selection. Disabling Easy Communication restored mouse interaction but removed convenient automatic radio-frequency tuning.

### Testing

- F-14 with Easy Communication enabled: menu opened, mouse selection failed.
- F/A-18C under the same mission conditions: mouse selection worked.
- F-14 after pressing the bound **Tomcat Ball** command once: mouse selection immediately worked.

### Decision

Force **Easy Communication ON** in the development mission.

### Reason

The squadron benefits from automatic radio tuning, particularly for casual and new players. The one-button Tomcat Ball workaround is less disruptive than requiring routine manual radio tuning.

### Player procedure

After spawning in the F-14, press the bound **Tomcat Ball** command once, then verify the communications menu accepts mouse input.

### Related documentation

- `docs/known-issues/f14-comms-menu.md`
- `docs/baseline-dcs-settings.md`
- `docs/new-player-checklist.md`

## 2026-08-06 — Zone-triggered opposing aircraft

### Change

The opposing aircraft group is configured to activate when any BLUE coalition unit enters the trigger zone named `MIGS`.

### Intent

Use coalition-based zone entry so the event is not tied to one specific player slot or aircraft group. This should allow the mission logic to work regardless of which allied player reaches the area first.

### Verification still required

- Confirm the group starts inactive or late-activated as intended.
- Confirm a BLUE aircraft entering `MIGS` activates the group.
- Confirm an unrelated coalition does not activate it.
- Confirm the trigger fires only once.
- Confirm the activated group follows its intended route and tasking.
- Confirm multiplayer clients observe the same result.

---

## Log entry template

```markdown
## YYYY-MM-DD — Change title

### Problem or objective

### Change

### Reason

### Test performed

### Result

### Follow-up
```

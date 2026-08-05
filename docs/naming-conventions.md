# Naming Conventions

Consistent names make Mission Editor logic, repository history and multiplayer troubleshooting easier to understand.

## Repository files

Use lowercase folder names and hyphenated Markdown file names.

Examples:

```text
docs/mission-standards.md
assets/briefings/
scripts/custom/
```

## Mission files

Recommended format:

```text
SSO-<map>-<mission-name>-v<major>.<minor>.miz
```

Examples:

```text
SSO-Syria-Base-Template-v0.1.miz
SSO-Syria-Coastal-Strike-v1.0.miz
SSO-Persian-Gulf-Tanker-War-v1.2.miz
```

Use `v0.x` for development and test versions. Use `v1.0` when a mission has completed the release checklist.

## Mission Editor groups

Recommended pattern:

```text
<coalition>-<role>-<number>-<description>
```

Examples:

```text
BLU-PLAYER-01-F14
BLU-CVBG-01-CARRIER
BLU-AWACS-01
BLU-TANKER-01-RECOVERY
RED-CAP-01-MIG29
RED-SAM-01-SA10
RED-TARGET-01-DEPOT
NEU-CIV-01-TRANSPORT
```

## Units

Where useful, append a two-digit unit number:

```text
BLU-PLAYER-01-F14-01
BLU-PLAYER-01-F14-02
RED-CAP-01-MIG29-01
```

Do not retain generic names such as `New Airplane Group #017` in a release mission.

## Trigger zones

Recommended pattern:

```text
ZONE-<purpose>-<location>
```

Examples:

```text
ZONE-TRIGGER-TARGET-AREA
ZONE-WEAPON-SAFE-CARRIER
ZONE-CAP-NORTH
ZONE-RECOVERY-CARRIER
```

## Triggers

Recommended pattern:

```text
<phase>-<sequence>-<action>
```

Examples:

```text
INIT-010-LOAD-SCRIPTS
START-020-WELCOME-MESSAGE
INGRESS-100-ACTIVATE-RED-CAP
TARGET-200-CHECK-DEPOT-DESTROYED
EGRESS-300-ENABLE-RECOVERY
END-900-MISSION-SUCCESS
```

Using sequence numbers leaves room to insert additional logic later.

## Flags

Prefer named flags where supported by the chosen scripting framework. If numeric flags are used, reserve blocks by purpose and document them.

Suggested blocks:

| Range | Purpose |
|---:|---|
| 1–99 | Initialisation and global state |
| 100–199 | Player and package state |
| 200–299 | Primary objective |
| 300–399 | Secondary objectives |
| 400–499 | AI activation and threat state |
| 500–599 | Radio menu |
| 900–999 | Mission completion and debug |

## Lua scripts

Use lowercase hyphenated or underscored file names consistently within a mission.

Examples:

```text
mission-init.lua
carrier-support.lua
radio_menu.lua
```

## Assets

Include the mission or template name when an asset is not globally reusable.

Examples:

```text
syria-coastal-strike-briefing-01.png
syria-base-template-radio-card.png
mission-001-awacs-intro.ogg
```

## Commit messages

Use short, action-oriented descriptions:

```text
Add Syria carrier template
Correct recovery tanker TACAN
Document F-14 radio presets
Test multiplayer success triggers
```

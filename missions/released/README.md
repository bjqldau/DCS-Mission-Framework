# Released missions

Only **verified, multiplayer-tested** mission builds go here. This folder is deliberately empty of `.miz` files until a release is confirmed.

Release procedure:

1. Test the exact development `.miz` build end-to-end, including multiplayer joining, player slots, triggers, radio menus, objectives and mission completion/recovery.
2. Copy its binary unchanged from `../development/` into this directory. Never silently modify an existing release.
3. Move any previous released build into `../archive/<mission>/`.
4. Record version, date, test evidence, known issues and release notes in a commit and preferably a mission-specific Git tag.
5. Share only the artifact from this folder with players.

Keep one current released `.miz` per mission; Git history and `../archive/` retain older versions. A version number alone does **not** prove release status.

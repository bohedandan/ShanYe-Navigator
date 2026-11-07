# ShanYe Navigator 3.0.7 RC4

This update focuses on loading and expanded-session stability.

- Fixed the single-player initialization path being expanded from one slot to sixteen. The project owner confirmed that entering the single-player map works after this fix.
- Replaced the rejected 37-entry expanded player dictionary with the original 17-entry layout and restored 16 internal player slots.
- Limited expanded-session settings to 8 or 16 players. All peers must update and the host must create a new room.
- Removed convoy voice in this release line while retaining shared control messaging and existing settings.
- Included the installation/update manager, English instructions, credits and original licenses.

## Validation

Managed builds, reference checks, 314 local capacity/layout fixture checks, archive integrity and isolated installation/update/uninstall checks passed. The RC4 package was installed on the project owner's machine and single-player loading was confirmed working.

**Not yet accepted:** real full 16-player sessions, cross-machine synchronization, late-join interactions and long multiplayer sessions. Local fixtures do not replace real-player testing.

Replace the RC1/RC2/RC3 test packages with this RC4 build. This is a prerelease, not a fully accepted stable release.

## Install

Exit the game, extract the complete ZIP, open ShanYe-Manager.exe, select/detect the game folder, choose Install / Update and start the game through Steam. Keep the accompanying program folder beside the manager. See README.txt in the ZIP for details.

Game build: 26.10.30_426818b / Steam 26326013. Loader: BepInEx x64. Revision: 20261108-rc4-singleplayer.

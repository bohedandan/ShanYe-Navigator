# In-menu help candidate - November 10, 2026

ShanYe Navigator 3.0.7 RC4 - In-menu help update
November 10, 2026 | Candidate revision: 20261110-rc4-help1

Added How to use on all 11 feature pages. Read the current page or search all help entries in English or Chinese. Selecting a tuning item first focuses its instructions. Use Back to controls or Esc to return without changing the previous page's scroll position.

The guide contains 60 topic summaries and 142 tuning-catalogue entries. It explains the steps, parking requirements, host/client permissions and saved-progress effects. Unavailable entries are explicitly marked. These are 202 help entries, not 202 independently validated features.

Existing RC4 users must run Install / Update to receive the help update. The offline Unity cache and installer remain included and unchanged. This update does not change gameplay, multiplayer protocol, configuration format or dependencies.

Validation: builds and 791 game/Unity references passed, alongside isolated help checks, menu geometry, archive integrity and synthetic install/update/uninstall checks. Installed on the project owner's machine with existing settings and save-file hashes preserved. Actual in-game help rendering/input and full 16-player acceptance remain pending.

Known limitation: tuning-preset import currently lacks a file-path input; the guide identifies this rather than claiming it works. Existing save/load/export actions are separate.

BepInEx x64; game build 26.10.30_426818b / Steam build 26326013.
Voice, text chat and whole-vehicle scaling remain removed; accessory scaling is retained.


---

RC4 offline-library packaging update - 2026-11-09

The installer validates versioned dependencies from its package metadata: Unity engine version, required archive modules, loader/runtime/plugin presence and hashes, and loader cache/source compatibility. Custom cache/source configurations are reported before any changes, rather than overwritten. The manager no longer treats a matching main DLL as proof that dependencies are healthy.

This complete installer includes the Unity 6000.0.75 base-library archive. Install / Update copies it to BepInEx/unity-libs/6000.0.75.zip and repairs missing or damaged copies. With the normal BepInEx cache/source configuration, the loader uses this file instead of downloading it on first startup.

Exit the game, fully extract this package and run ShanYe-Manager.exe -> Install / Update, even if RC4 is already installed. No separate repair package is needed. Keep the inner Unity ZIP intact. Interface generation still runs and can take time.

Mod/loader binaries, game fingerprint checks, saved settings and multiplayer protocol are unchanged. Custom loader cache/source paths may need separate review. This removes one Unity-library download dependency; Steam/multiplayer and unrelated services still require their usual connectivity.

The libraries come from the known working local BepInEx cache. ZIP integrity and all 73 extracted DLLs were checked. The matching loader's cached-library method passed isolated checks. Startup on the affected player's machine and full 16-player multiplayer acceptance remain pending.

Original endpoint: https://unity.bepinex.dev/libraries/6000.0.75.zip
Archive SHA256: 53C15D574B129486F71F93825677983787E7242AED98D083D3DB93B87A985655
Unity/BepInEx materials retain their respective rights and terms. Existing package licenses/notices remain applicable.


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

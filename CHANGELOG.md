# ShanYe Navigator 3.0.8 RC2

For Over the Hill **26.11.06_db90b37 / Steam build 26489201**, Windows x64, BepInEx only.
Revision: **20261114-rc2-menu-input**. This is a prerelease.

## Changes

- Updated room-creation hooks for the new game network library. Kept the official networking library and the existing 8/16-player options; ordinary four-player mode remains available.
- Added 29 searchable release-history entries in English and Chinese. Open Display & Settings > Display & Keys and scroll to the bottom.
- Added a recognizable bilingual installer filename and ShanYe icon. Main buttons show Chinese and English.
- Fixed the missing tuning-preset name/path inputs. Invalid files are rejected before saving; importing does not apply settings to the vehicle.
- Added native UI pointer isolation while the mod menu is open after finding that language-dialog clicks could also select a map in the background.
- Kept the matching offline Unity library cache, saved preferences and existing accessory presets.

## Install or update

Exit the game, extract the complete ZIP and run **山野领航-安装更新卸载-ShanYe-Setup.exe**. Keep the adjacent **程序文件** folder. Detect/browse to the folder containing `over the hill.exe`, choose **Install / Update**, and start through Steam. Existing users should update directly; do not uninstall first.

Default keys: **Insert** for the menu, **End** to disable the mod, **Ctrl+F5** for the FPS optimizer. Saved bindings take precedence. Select **English / 中文** at the top of the menu. Do not use **Back up & delete** for an ordinary update: that option clears game progress.

## Validation and limits

The current revision passed local English/Chinese release-history display, version search/clear, same-language return position, language-dialog click-through and native-button recovery checks. The installer icon, bilingual labels, automatic path detection and running-game preview refusal were observed. The original Chinese language preference was restored. This is one-machine UI validation, not multiplayer acceptance.

Local x64 build, native reference/target checks, production-code input/help fixtures, archive integrity and isolated installation/upgrade checks passed. Test doubles and synthetic directories do not establish multiplayer behavior. Real 4/8/16-player sessions, late joining, reconnection, cross-machine appearance/gathering/gear synchronization, and extended driving remain unverified in this task. No real multiplayer participant count was accepted.

All players in an expanded room should use this package. The host selects capacity outside a room, then creates a new room. A client's setting cannot expand the host's room.

Voice, text chat and whole-vehicle scaling remain removed. Accessory position, rotation and scaling remain available. Older releases are preserved for their supported game builds.

## Credits and feedback

Menu and integration: **Danjuan Erwang (蛋卷儿王)**. FPS optimizer: **Putao Ban Dasuan (葡萄拌大蒜)**. Real Nights and Lights: **SquidFromWish**. Hydraulics: **Jonathon**. OverTheHillUnlimited: **t04glovern / Nathan Glover**. ExtraGears reference/adaptation: **kaleLetendre**. Original licences and further notices are included; this is a binary-distribution project, not an open-source licence grant.

Report bugs in this repository's Issues with the game/mod version, role, player count, steps and screenshot. For crashes, attach `BepInEx/LogOutput.log` after checking it for private names and local paths. Do not upload credentials or personal saves.


---

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

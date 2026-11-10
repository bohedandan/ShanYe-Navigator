# ShanYe Navigator

A community-made utility mod for **Over the Hill** (also written as **OverTheHill**), by **Danjuan Erwang (蛋卷儿王)**. ShanYe Navigator is known as **山野领航** in Chinese.

## Download

**[Download 3.0.7 RC4 with in-menu help](https://github.com/bohedandan/ShanYe-Navigator/releases/tag/v3.0.7-rc4)** · **[Report a bug](https://github.com/bohedandan/ShanYe-Navigator/issues)**

Download the complete ZIP from this repository's **[Releases](https://github.com/bohedandan/ShanYe-Navigator/releases)** page. Choose `ShanYe-Navigator-3.0.7-RC4-Help1-Offline-BepInEx-x64.zip`, not GitHub's automatic source-code archives.

**3.0.7 RC4 is a prerelease.** Single-player loading has been confirmed working by the project owner after the fix. Full 16-player multiplayer acceptance is still pending.

## In-menu help update (November 10, 2026)

Every feature page now has **How to use** at the top. Read instructions for the current page or search all help in English or Chinese. Select a tuning item before opening help to focus its instructions. Use **Back to controls** or **Esc** to return to the previous page position.

The guide includes **60 topic summaries and 142 tuning-catalogue entries**. It explains steps, parking requirements, host/client permissions and saved-progress effects. Unavailable entries are marked; this is not a claim of 202 verified features. The complete English guide is also included as `FEATURE-GUIDE.txt` in the ZIP and as a release attachment.

Existing RC4 users need to run **Install / Update** to receive this help update. The offline cache remains included. Gameplay logic, the multiplayer protocol, settings format, dependencies and installer are unchanged.

This candidate is revision **20261110-rc4-help1**. Build, reference, isolated help/layout and installation checks passed. It was installed on the project owner's machine with settings and save-file hashes preserved. **Actual in-game help rendering/input remains unverified.** Full 16-player acceptance is still pending.

## Offline-ready installer update (November 9, 2026)

The recommended complete ZIP now includes the matching Unity base-library cache. This addresses first-start failures while downloading Unity libraries, followed by UnityEngine.CoreModule not found.

Run **Install / Update again**, even if RC4 is already installed. The installer checks the package's declared Unity version, required offline modules, loader/runtime/plugin requirements and package hashes, and repairs missing or damaged distributed files. Previously saved loader configuration is retained. Custom cache/source settings that bypass the bundled archive are reported before installation rather than silently overwritten.

No separate Unity repair archive is needed. Do not unpack the inner Unity ZIP. Normal first-start interop generation still takes time. This is not an offline multiplayer mode, and startup on the affected player's machine is still awaiting confirmation.

## Requirements

- Windows x64 and Over the Hill build **26.10.30_426818b** (Steam build **26326013**).
- This package includes the BepInEx x64 loader and required distribution files.
- BepInEx is the supported loader for this release. Do not install two loaders together.

## Install or update

1. Exit the game.
2. Extract the entire ZIP to a folder. Do not run the manager from inside the archive.
3. Open **ShanYe-Manager.exe**. Keep the accompanying `程序文件` folder beside it; its name is required by the installer.
4. Let the manager detect the game, or browse to the folder containing `over the hill.exe`.
5. Click **Install / Update** and wait for completion, then start the game through Steam.

The same button supports first installation and updates. Existing language, key bindings, HUD preferences and appearance presets are retained. If the installer reports an unsupported game build, report the message rather than forcing files into place.

The manager and in-game menu include English. Select **English / 中文** at the top of the menu. Internal package names and original legal notices are retained for compatibility and attribution.

## Main tools

- Searchable in-menu instructions for each feature page, in English and Chinese.
- Minimap, player markers, driving instruments, FPS and latency display.
- Portable mechanic, saved-vehicle switching, owned accessories and installed community liveries.
- Accessory stacking, layout editing, copies and saved presets.
- Transmission tuning, manual neutral and related vehicle options.
- Multiplayer tools, gathering requests and configurable expanded sessions.
- Weather/time controls, accessory lighting, night settings, hydraulics and performance options.
- Configurable keyboard/controller bindings and saved preferences.

Availability depends on the current scene, ownership, host permissions and enabled settings. Multiplayer synchronization and late-join interactions still require cross-machine testing. Voice and text chat are not included. Whole-vehicle scaling is not included; accessory scaling remains available.

## Default shortcuts

| Key | Action |
| --- | --- |
| Insert | Open or close the menu |
| End | Disable the mod |
| Ctrl + F5 | Toggle the FPS optimizer |

Previously saved custom bindings take precedence. Other bindings can be reviewed in the display/settings section. Stop the vehicle before changing vehicles, accessories or tuning.

## Expanded multiplayer

The configuration supports **8 or 16 players**, with a maximum of 16. Ordinary four-player mode remains available.

All participants must use this candidate build. The host must enable expansion and select the limit **outside a room**, then create a new room. Changing client settings does not expand an existing host's room. Older expansion layouts are not compatible.

The 16-player setting is not a claim that a full 16-player session has passed acceptance. Test joining, photo spots, mechanics, camps, gathering, transmission approvals, appearance synchronization, late joins, reconnects and map changes. Report the host's and client's versions and roles.

## Uninstall and save backup

Exit the game, run the manager and choose **Uninstall**. Save backup is available separately. **Back up & delete** removes local game progress and is not needed for normal installation, updating or uninstalling. Only the latest save backup is retained.

## Report a problem

Open an issue with the mod version, game build, single-player/host/client role, player count, steps and a screenshot. For crashes or loading problems, include `BepInEx/LogOutput.log` from the game directory. Review logs for private names and local paths before posting. Mention other installed mods.

## Credits and license

- Menu, original features and integration: **Danjuan Erwang (蛋卷儿王)**.
- OVH Render Optimizer: **Putao Ban Dasuan (葡萄拌大蒜)**.
- Real Nights and Lights: **SquidFromWish**.
- Hydraulics: **Jonathon**.
- OverTheHillUnlimited: **t04glovern / Nathan Glover**.
- ExtraGears reference/adaptation: **kaleLetendre**.
- BepInEx, MinHook and other dependencies retain their original authorship and licenses.

Original portions are distributed under the included **ShanYe Navigator Personal Use License 1.0**. This is a binary-distribution repository, not an open-source license grant. Third-party licenses remain applicable; full notices are included in the package. This is an unofficial mod and is not affiliated with the game developers or Steam.

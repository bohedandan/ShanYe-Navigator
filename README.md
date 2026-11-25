# ShanYe Navigator

A community-made utility mod for **Over the Hill** (also written as **OverTheHill**), by **Danjuan Erwang (蛋卷儿王)**. ShanYe Navigator is known as **山野领航** in Chinese.

## Download

**3.0.9 RC1** is the Windows x64 prerelease for Over the Hill **26.11.19_CB94FA2**, Steam build **26790649**. The full ZIP includes the bilingual installer, BepInEx and the matching offline Unity libraries. [Download the full ZIP](https://github.com/bohedandan/ShanYe-Navigator/releases/download/v3.0.9-rc1/ShanYe-Navigator-3.0.9-RC1-Offline-BepInEx-x64.zip) · [Release notes and checksums](https://github.com/bohedandan/ShanYe-Navigator/releases/tag/v3.0.9-rc1)

Running an older game build? Each previous release lists the build it supports. [All releases](https://github.com/bohedandan/ShanYe-Navigator/releases)

## What's new in 3.0.9 RC1

- The game sets the room limit. This release removes the expansion plugin, its controls and its shortcuts. Team gathering, gear approvals and accessory and paint sharing remain available in native rooms.
- Inventory, currency and saving now use the updated game's profile data. In-game backups follow the active account once the game's save migration finishes. The installer lists both Steam account saves and legacy locations and asks you to choose when it finds more than one.
- Hydraulics now reads the profile name from its new location.

Tested on one Windows PC by updating from 3.0.8 RC2, launching through Steam and entering Emerald Lake in single player. The vehicle, minimap and dashboard appeared. Both the team menu and the home shortcuts were checked for removal of the expansion controls. Extended driving, live hydraulics and cross-PC multiplayer still need player testing. The revision tested was `20261126-rc1-native-rooms`.

## Feature instructions

Every feature page has **How to use** at the top. Read the current page or search all help in English or Chinese. Select a tuning item before opening help to focus its instructions. Use **Back to controls** or **Esc** to return to the previous page position.

The English feature guide covers 58 topics and 142 tuning entries. The release history covers 30 versions and revisions. Both are downloadable on the release page and searchable in the mod in English or Chinese.

## Requirements

- Windows x64 and Over the Hill build **26.11.19_CB94FA2** (Steam build **26790649**).
- This package includes the BepInEx x64 loader and required distribution files.
- BepInEx is the supported loader for this release. Do not install two loaders together.

## Install or update

1. Exit the game.
2. Extract the entire ZIP to a folder. Do not run the manager from inside the archive.
3. Open **山野领航-安装更新卸载-ShanYe-Setup.exe** (the installer with the ShanYe icon). Keep the accompanying `程序文件` folder beside it; its name is required by the installer.
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
- Native-room team tools, gathering requests, gear approvals and accessory and paint sharing.
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

## Multiplayer

Create and join rooms through the game's own multiplayer menu. Update the host and teammates to the same helper release to use gathering, gear approvals and appearance sharing. The updater removes the expansion plugin shipped with earlier versions. Use a native room for RC1 sessions.

## Uninstall and save backup

Exit the game, run the manager and choose **Uninstall**. Save backup is available separately. **Back up & delete** removes local game progress and is not needed for normal installation, updating or uninstalling. Only the latest save backup is retained.

## Report a problem

Open an issue with the mod version, game build, single-player/host/client role, player count, steps and a screenshot. For crashes or loading problems, include `BepInEx/LogOutput.log` from the game directory. Review logs for private names and local paths before posting. Mention other installed mods.

## Credits and license

- Menu, original features and integration: **Danjuan Erwang (蛋卷儿王)**.
- OVH Render Optimizer: **Putao Ban Dasuan (葡萄拌大蒜)**.
- Real Nights and Lights: **SquidFromWish**.
- Hydraulics: **Jonathon**.
- Earlier releases used OverTheHillUnlimited by **t04glovern / Nathan Glover**.
- ExtraGears reference/adaptation: **kaleLetendre**.
- BepInEx, MinHook and other dependencies retain their original authorship and licenses.

Original portions are distributed under the included **ShanYe Navigator Personal Use License 1.0**. This is a binary-distribution repository, not an open-source license grant. Third-party licenses remain applicable; full notices are included in the package. This is an unofficial mod and is not affiliated with the game developers or Steam.

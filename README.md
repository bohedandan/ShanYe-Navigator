# ShanYe Navigator

A community-made utility mod for **Over the Hill** (also written as **OverTheHill**), by **Danjuan Erwang (蛋卷儿王)**. ShanYe Navigator is known as **山野领航** in Chinese.

## Download

**[Download 3.0.8 RC2](https://github.com/bohedandan/ShanYe-Navigator/releases/tag/v3.0.8-rc2)** · **[Report a bug](https://github.com/bohedandan/ShanYe-Navigator/issues)**

Choose `ShanYe-Navigator-3.0.8-RC2-Offline-BepInEx-x64.zip` from **Releases**, not GitHub's automatic source-code archives. This is a prerelease for game **26.11.06_db90b37 / Steam 26489201**. Use the older RC4 package only with its supported older game build.

## What's new in 3.0.8 RC2

- Adapts the room-creation hooks to the game's updated network library while retaining the official networking changes. Maximum expansion remains 16 players.
- Adds searchable, bilingual release history at the bottom of **Display & Settings > Display & Keys**, covering 29 retained release records from 2.5.2 onward. Historical features are not a current feature list.
- Makes the installer easier to find: a Chinese/English filename, the ShanYe icon and bilingual buttons. First installation and updating use the same entry.
- Adds the missing tuning-preset name and JSON-path inputs, with format, value-range and 1 MB checks before saving. Import does not apply a preset to the vehicle.
- Isolates native UI pointer targets while the mod menu is visible, addressing language-dialog clicks reaching map-selection buttons behind it.

Revision: **20261114-rc2-menu-input**. The current revision passed local English/Chinese release-history display, version search/clear, same-language return position, language-dialog click-through and native-button recovery checks. The installer icon, bilingual labels, automatic path detection and running-game preview refusal were observed. The original Chinese language preference was restored. This is one-machine UI validation, not multiplayer acceptance.

The package includes the loader and matching offline Unity base libraries. Normal first-start interface generation still takes time. Full 16-player multiplayer acceptance remains pending.

## Feature instructions

Every feature page has **How to use** at the top. Read the current page or search all help in English or Chinese. Select a tuning item before opening help to focus its instructions. Use **Back to controls** or **Esc** to return to the previous page position.

The guide includes 60 topic summaries and 142 tuning-catalogue entries explaining steps, parking, host/client permissions and saved-data effects. These are help entries, not 202 independently validated features. An English `FEATURE-GUIDE.txt` and `RELEASE-HISTORY.txt` are included as release assets.

## Requirements

- Windows x64 and Over the Hill build **26.11.06_db90b37** (Steam build **26489201**).
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

---
date: 2016-08-06
title: Space Jawns v2.1.1 Alpha is available!
categories:
  - release
  - game news
author_staff_member: sk33lz
---

I've made some huge advancements in the subsystems of the game in this release. I have also been able to start adding some new content as some of the systems are starting to settle in. There is a new "set it and forget it" style high score submission system that prompts you the first time you play, and will save your name and High Score to compete for the Global High Score online. THere are a bunch of other fixes and improvements in the Changelog. Check it out!

## Changelog
- Fixed menu selection issues with keyboard, gamepad, and joystick.
- Added menu selection sounds when selecting with keyboard, gamepad, and joystick.
- Added source code to git repository for easier code changes and reverting.
- Setup new Save High Scores for set it and forget it. After set, can change settings from options page.
- Set version number after build programatically using assembly versioning. Creates a file and imports data on main menu.
- Added new turret asset.
  - **Add Credits
  - Author: Phex3D
  - Link: https://www.assetstore.unity3d.com/en/#!/publisher/267
- Fixed turret logic. Enemy Turrets now follow the player's movement.
- Fixed enemy laser from firing in a vertical to firing in a horizontal rotation.
- Fixed high score system on Android devices.
- Fixed background music on main menu to start when game actually starts instead of script awake.
- Added Advanced Options menu page from Options page. Other menus may be added.
  - This page will have advanced options that don't belong on the main options page.
- Created text asset files instead of actual text files to handle versioning on Main Menu better on all platforms.
  - Will be moving some of the other static text assets during build into this system like Credits, Changelog, etc.
  - Seems buggy on Android, as the UI.Text has the original text asset data and has not updated.
- Added custom Splash Screen image.
- A few other fixes for Android and Standalone high scoring that were bugged due to a git revert with good changes in it.
  - High Scores got reset in the process on each device. This may happen again in other Alpha versions.
    - All Online High Scores should be safe. (Don't quote me on that.)
- Fixed Main Menu link on Credits page, as it was starting a new game instead of going to Main Menu screen.

Check out the [Space Jawns download](/download) page to get the latest files.

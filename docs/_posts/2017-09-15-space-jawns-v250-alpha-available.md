---
date: 2017-09-15
title: Space Jawns v2.5.0 Alpha is Available!
categories:
  - release
  - game news
author_staff_member: sk33lz
---

The latest installment of Space Jawns, version 2.5.0, is now available. This update includes changes from many smaller updates and changes many mechanics of the game. Because of this, we have reset the player high scores both locally and online. You must upgrade to Space Jawns 2.5.0 Alpha to register to submit your high scores online again. See the full changelog on the download page for all the new changes. Good luck and have fun!

This release is actually a handful of smaller releases wrapped into a massive release. I'm the only developer on this project with a bunch of friends helping me debug problems with the game, so packaging up a ton of files for a small amount of changes is not very efficient for me. This release fixes a ton of bugs, adds a ton of new functionality, and resets the high scores. See the changelog for full list of changes.

## Changelog
- Continued adding Career Stats to the Pilot Profile.
  - Pilots now track career stats totals for:
    - Total Enemy Ships
    - Total Asteroids
    - Total Playing Time
  - These Career Stats need to be added:
    - Total Powerups
    - Total Bonuses
    - Total Max Level
    - Total Player Ships Used
    - Total Levels Completed
- Tried some changes to texture baking, but didn't see much difference, so reverted.
- Fixed issue with FPS toggle not working properly and displaying wrong value.
- Finally fixed enemy laser physics!
- Added point bonus targets. Shoot flying fruit to gain bonus points.
- Removed a bunch of old code and debug code from scripts that have been ironed out.
- Limited firing range of enemy turrets so they don't shoot you from behind.
- Enemy ships are now destroyed if they leave the playing area, so they no longer circle back and attack again.
- Completed dymanic difficult level based on current level number and difficulty setting in options.
- Started adding all sounds to new sound mixer controls. Next is to connect it to the main volume setting in options for testing.
- Continued work on dynamic fire rates and other variables to allow for better powerups and dynamically changing gameplay elements on the fly.
- Various small tweaks and bug fixes to enemy ship physics and enemy turret physics.
- Forcing auto-fire off on game load until bugs are fixed with mobile.
- Added new explosion animations and sound FX for powerups and bonuses.
- Fixed issue with resetting to main menu from pause menu not resetting to level 1 start values.
- Added new soundFX and fixed more small issues for 2.5 launch.
- Tweaked new powerups to ensure they work and disable at right times.
- Added dynamic dificulty level that changes based on current level. Other settings will be based off this value.
- Fixed a bunch of issues introduced by new powerups and bonuses.
- Fixed a bunch of other small bugs and issues that have been overshadowed by the enemy laser physics.
- Stats have been forced reset due to changes to many scoring elements and addition of lifetime stats.

Check out the [Space Jawns download](/download) page to get the latest files for your device.

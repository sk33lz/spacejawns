---
date: 2019-03-05
title: Space Jawns v3.0.0 Alpha is Available!
categories:
  - release
  - game news
author_staff_member: sk33lz
---

Space Jawns version 3.0.0 Alpha is available now for [download](/download) for Windows, MacOS, Linux, and Android! 

I've been working hard on the latest Space Jawns release for over a year now. It's gone from version 2.5.1 all the way to version 3.0.0 with this release. There are a ton of fixes, new features, and lots of Unity version upgrades over that time. Our most recent spring was getting the game updated to Unity 2018.3.6. See all the changes since the last release included in Space Jawns 3.0.0 Alpha below!

## Changelog

## 3.0.0-Alpha
- Made base game resolution 1920x1080 instead of 1024x768 pixels.
- Fixed several UI issues that came from changing base resolution.
- Started making UI buttons much bigger to match the new base resolution.
- Upgraded to Unity 2017.4.18f1 LTS.
- Fixed a few warnings of deprecated Unity code after Unity 2017.4.18f1 upgrade.
- Upgraded to Unity 2018.3.1f1.
- Fixed additional warnings of deprecated Unity code after 2018.3.1f1 upgrade.
- Updated all deprecated WWW class code to new UnityWebRequest class.
- Upgraded to Unity 2018.3.6f1.s

## 2.6.1-Alpha
- Upgraded to Unity 2017.1.2. It was a pretty clean upgrade aside from a single deprecation warning.
- Fixed input caret on login fields not lining up properly.
- Fixed Space Jawns Configuration/Launch image size so it's readable.
- Added Password Reset and email validation on Register.
- Added Register from multiple accounts on a single device.
- Security Audit and fixes to new login system. Thanks Nick!
- Lots of other bug fixes and enhancements.
- Fixed issue with deadzone toggle on Android.
- Fixed username profanity filter.
- Verified COPPA compliance for registration.
- Added pitch variations to sound FX that are repetitive to give them some ear candy.
- Fixed lasers missing most asteroids.
- Started working on sound mixers for music, sound FX, and menus.
- Reduced turret shooting radius.
- Reduced turret difficulty.

## v2.6.0-Alpha (Old v2.5.1-Alpha, v2.5.2-Alpha & v2.5.3-Alpha)
- Upgraded to Unity 5.4.1. Debugged several issues related to that process.
- Saving player name for online high scores choices have been moved to start of game for easier usage.
- Fixed a bunch of small issues with the UI like default values being 999999999 instead of 0.
- Changed how Energy Bonus Powerup works. They now add 25 max energy for a short time.
- Added visual border at the edge of the playable area for larger screen resolutions.
- Fixed some issues with other powerups stats not applying correctly, or that had blinking powerup UI messages.
- Added additional sound FX for powerups; Energy Bonus, Energy Recharge, Extra Ship, and Laser Upgrade.
- Changed gameplay width to be equal for all player screen widths instead of based on screen width.
- Fixed some lighting issues with Android gameplay from 2.5.0 update. Thanks Henrik!
- Moved some of the more unused options to the Advanced Options page. We'll see how it goes.
- Did some optimization attempts for textures and sprites on Android. Hoping for better all around performance!
- Local player stats have been wiped on this update, but the online high scores are staying as is.
- Started adding new player account login system. Still needs work, but is working at the lowest level currently and allows signups.
- High Scores for Standalone vs. Android are saved separately, so that we can see what platforms score higher.
- Started adding tab key navigation to menu system. Forward with tab, backward with shift + tab.
- Added in-game console to display log messages. Press the tilda key "~" to access the console.
- Added additional career stats to new login system.
- Upgraded to Unity 5.6.0.
- Added quick startup screen to Just Play, Login, Register, or Quit.
- Pressing enter after entering your password when on the login screen now logs you in.
- Just Play sets the player name to Player 1.
- Just Play resets saved data from the last login except for the last local device high score. Challenge your friends without messing with your user.
- Improved some Powerup messages.
- Added career stats tracking for Powerups and Bonuses.

Check out the [Space Jawns download](/download) page to get the latest files for your device.

Found a bug? Report it to [Space Jawns Support](/support) on Discord!

---
date: 2015-04-08
title: Space Jawns v2.0.7 Alpha is available!
categories:
  - release
  - game news
author_staff_member: sk33lz
---

It took longer than I thought it would, over a month, but I have compelted migrating all of the legacy Unity GUI elements to the new Unity 4.6+ UI element. Using both systems together has been causing some odd display issues on different devices. The new UI system introduced in Unity 4.6 scales much better than the legacy GUI system from my testing, and that's what made me want to update all of the elements to the UI system in the first place. There are many other enhancements that went into this relase like new custom sound effects and visual effects. See the full Changelog for the 2.0.7 Alpha release below.

## Changelog Alpha 2.0.7 - 4/8/15
- Set default orientation on mobile devices to Landscape mode only and disabled Portrait mode.
- Added deadzone for Android accelerometer so ship comes to a complete stop when almost centered.
- Added some smoothing to Android accelerometer input to make movements less jumpy.
- Debugging sound and UI issues between devices and resolutions.
- Updated all legacy GUI elements to Unity 4.6+ UI elements on all menus and game interfaces.
- Added additional silly text, "Now With Added Butter!".
- Moved scores DB off test server to better server to avoid offline errors.
- Make sure Top100 page is mobile responsive.
- Add column headings for High Score table.
- Added online high score stats data for Device Type and Platform. This data will be used to categorize high scores.
- Added ability to save and load a game save files on most supported devices.
  - See http://spacejawns.com/about/how-play#backup
- Added ability to select menu items with arrow keys or gamepad/joystick.
- Removed ship explosion sound effect, Explosion.wav.
- Added custom sound effect created in Bfxr standalone program for ship explosion.
  - Explosion1985.wav
- Added custom sound effect created in Bfxr standalone program for asteroid explosion.
  - short-explosion.wav
- Added custom asteroid explosion visual effect from modified standard assets fireworks effect.
- Removed Final death sound effect, Retro_Game_Sounds_SFX_85.wav.
- Added custom sound effect created in Bfxr standalone program for Final death sound effect
  - sj-final-death.wav.
- Compressed all sound fx to ogg vorbis with highest compression as we are going for raw sound fx anyway.
- Added play game button to Pause menu to allow unpausing from the menu. This option is selected by default.

Check out the [Space Jawns download](/download) page to get the latest files.

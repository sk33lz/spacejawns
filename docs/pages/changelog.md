---
title: Changelog
permalink: /game/changelog
heading: Space Jawns Changelog
description: Here you can you find every change that I could remember while making the game so far.
---

## Alpha 2.5.0 - 09/15/17
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
- Completed dynamic difficult level based on current level number and difficulty setting in options.
- Started adding all sounds to new sound mixer controls. Next is to connect it to the main volume setting in options for testing.
- Continued work on dynamic fire rates and other variables to allow for better powerups and dynamically changing gameplay elements on the fly.
- Various small tweaks and bug fixes to enemy ship physics and enemy turret physics.
- Forcing auto-fire off on game load until bugs are fixed with mobile.
- Added new explosion animations and sound FX for powerups and bonuses.
- Fixed issue with resetting to main menu from pause menu not resetting to level 1 start values.
- Added new soundFX and fixed more small issues for 2.5 launch.
- Tweaked new powerups to ensure they work and disable at right times.
- Added dynamic difficulty level that changes based on current level. Other settings will be based off this value.
- Fixed a bunch of issues introduced by new powerups and bonuses.
- Fixed a bunch of other small bugs and issues that have been overshadowed by the enemy laser physics.
- Stats have been forced reset due to changes to many scoring elements and addition of lifetime stats.

## Alpha 2.4.1 - 01/17/16
The 2.4.1-Alpha release is a bug fix release. Players were having issues saving their names for their high scores, and this update fixes that bug. Players should be prompted to save their name when they start the game, and once their score refreshes on the site it will update their saved name.

## Alpha 2.4.0 - 10/15/15
- Converted all game scripts from Javascript to C#.
- Fixed a bunch of small issues related to the C# migration.
- Converted all game scripts and assets to Unity 5.
- Fixed some small issues after Unity 5 migration with warnings and errors.
- Enlarged the skybox images to 2048x2048 for standalone platform.
- Removed game timer clock as it is being refactored for a goalTimer on certain levels.
- Original game timer clock has been turned into a new total time played career stat.
- Set asteroids to fixed sizes of small, medium, large, and huge to save on performance hits from previous method.
- Added Pilot Profile screen to track all career player stats on a specific player device.
- Started adding Career Stats to the Pilot Profile.
  - These Career Stats will be used to populate and track online player profile values for a given GUID.
    - Added Total Enemy Ships Destroyed.
    - Added Total Asteroids Mined.
    - Added Total Turrets Destroyed.
    - Added Total Time Played.
- Enemy Turrets and Enemy Ships have better rotation logic to track the player.
- Other small game tweaks and enhancements.

## Alpha 2.1.1 - 9/22/15
- Fixed menu selection issues with keyboard, gamepad, and joystick.
- Added menu selection sounds when selecting with keyboard, gamepad, and joystick.
- Added source code to git repository for easier code changes and reverting.
- Setup new Save High Scores for set it and forget it. After set, can change settings from options page.
- Set version number after build programatically using assembly versioning. Creates a file and imports data on main menu.
- Added new turret asset.
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

## Alpha 2.10 - 9/1/2015
- Enemy Turrets are aimed at right height now.
- Enemy Turrets now track player around the screen properly.
  - Set turretRotateError settings per level.
  - May need additional tweaking per level after QA.
- Tweaked dimensions for ultra-widescreen monitors. (Thanks Red!)

## Alpha 2.0.9 - 8/27/15
- Tweaking powerup settings.
  - Need to ensure only 1 powerup spawner is active at a time.
    - Maybe tag the spawner and ensure that gameobjects of that tag do not exist before another can be spawned.
- Added speed boost powerup for player ship speed.
- Added powerup message text to display powerup information when enabled/disabled.
- Fixed main menu selection while using a gamepad.

## Alpha 2.0.8 - 5/27/15
- Added player ship energy system that depletes as weapons are fired.
  - The goal will be to limit shots so that people can't just spam fire.
    - Level 1 lasers have a rated power usage of 25 units.
    - Level 1 ships have a total power rating of 100. This will allow for 4 shots before requiring more energy.
    - Gain power capacity through level up and temporary powerups.
- Higher level weapons will do more damage and use more energy.
- This will obviously need tweaking as levels progress, especially past level 10.
- Added energy bar UI component to display current energy level with percentage of energy level text label.
- Added levels 7-10 with added incremental difficulty levels. These may need tweaking.
- Added additional level of randomization for game objects. Now all spawners have their own random spawn points.
  - So far this includes enemy ships, asteroids, turrets, and powerups.
  - All spawns will have this randomization to keep the game content fresh every play.
  - May need some tweaking.
- Added custom skybox created with SpaceScape for Levels 3, 4, and 5. More custom skyboxes coming soon!
  - jNebula_Skybox
- Added some contrib skyboxes from Osirion pack re-exported in 4096px for Unity.
  - Added sky_26 for Levels 6, 7, and 8.
  - Added sky_08 for Levels 9 and 10.
- Added particle effects for enemy ship boosters.
- Added UI panel to background of game over totals.
- Added UI panel to background of online high scores.
- Added UI panel to background of session totals.
- Swapped out high poly asteroid for low poly asteroid.
- Added custom skin to low poly asteroid.
- Added random sizing of spawned asteroids.
- Added custom player and enemy laser1 materials.
- Removed old assets no longer in use and prefabs for old GUI components from game assets folder for spring cleaning.
- Cleaned up old code no longer being used from old GUI system.
- Limited player movement to just before countdown timer has completed to start the round.
- Limited player weapon firing until countdown timer has fully completed to start the round.
- Changed game time clock to start after round countdown timer has fully completed.
- Moved game time clock to top of screen and added a UI panel around it.
- Changed player ship laser color to green.
- Added custom powerup container model.
  - Each type of powerup will have it's own accent colors.
- Added timestamp for last submission time to global high scores.
- Added system identifier table for online high scores db and save info on submit.
- Added platform identifier table for online high scores db and save info on submit.
- Added timestamp, system identifier, and platform identifier to website api import data.
- Added UI button to View Online Credits page from in-game Credits screen.
- Added UI button to High Scores screen on Game Over screen menu.
- Optimized graphics and shaders for mobile. This should speed up all gameplay considerably.
- Created Options UI page that handles some game settings and saves them to player preferences.
  - Added Difficulty Level UI Slider with 4 Difficulty Levels and logic that controls overall difficulty.
  - Added Deadzone UI Toggle, disabled by default, but can be enabled to turn on a small deadzone for smoother, but slower control movements.
  - Volume Control UI Sliders are not functional yet.
  - Deadzone Angle UI Slider is not functional yet.
  - Add FPS UI Toggle, disabled by default, with FPS counter display on game HUD.
- Added UI button to Options Menu on Main Menu.

## Alpha 2.0.7 - 4/8/15
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

## Alpha 2.0.6 - 3/2/15
- Changed Main Menu to new UI Buttons instead of old GUI Button.
- Added scrolling Credits text.
- Fixed GUI elements overlapping on pause.
- Added 4th and 5th levels for additional testing of higher difficulty levels and awarding testers additional ships.
- Added silly random text to main menu screen.
- Added new High Score screen background music.
  - catinspace_h1.mp3
  - Credit: mutantleg
  - URL: http://opengameart.org/content/cat-in-space
- Added View Top 100 button on High Scores screen that opens browser to online high scores page.
- Redid most GUIText elements as UI.Text elements.
- Added opaque background to pause menu.
- Redid pause menu buttons as UI Buttons.
- Added a countdown timer for high scores submissions so that malicious users cannot hammer the database.
- Added incremental XP requirements IE: lvl1 2000 lvl2 3000 lvl3 4000 etc.
  - Added level scoring breakdown in README.txt
- Added limit to distance playerBullets can travel and damage enemies so it is harder to shoot enemies that are still off screen.

## Alpha 2.0.5 - 2/22/15
- Added ability to edit Player Name in High Scores system.
- Player Name is saved persistently in Player Prefs until edited.
- Player Name is displayed instead of Player 1 after saving a Player Name for High Scores.
- Fixed High Score Submit button type and placement.
- Fixed alignment on Top 10 High Scores so that they are centered, but in 2 even columns.
- Added versionNumber file to track version number instead of having to open up first scene to edit.

## Alpha 2.0.4 - 2/21/15
- Added global player high scores saved online.
  - Scores are saved in a database and top 10 are shown in game.
  - Top 100 scores will be shown on the website.
- Added GUID system for tracking unique players and devices in high score system.
- Added IP of player when posting high scores to allow possible user blocking of users who exploit the system.

## Alpha 2.0.3 - 2/9/15
- Added local player persistent high score counter. Tracks high score even after closing game.
- Added local player high score to High Scores page.
- Re-arranged player HUD and added player 1 score title and high score title.
- Fixed some bugs that popped up after adding turret count. Should be all fixed.

## Alpha 2.0.2 - 2/8/15
- Added custom sound effect created in Bfxr standalone program for game pause enable and disable.
  - pause-game.mp3
- Added custom sound effect created in Bfxr standalone program for player laser.
  - pew-pew-laser.mp3
- Added custom sound effect created in Bfxr standalone program for enemy laser.
  - pew-pew-laser-2.mp3
- Removed laser7.wav and Laser2.wav sounds in favor of new custom sounds created in Bfxr.
- Added custom menu select sound for all menu items.
  - select-long.mp3
- Removed select01.ogg in favor of new sound for all menu items.
- Added new mouseover menu item sound effect for all menu items.
  - mouseover-button.mp3
- Removed mouseover01.ogg sound in favor of new sound for all menu items.
- Added Paused UI text with menu items to return to main menu and quit game.
- Migrated 3, 2, 1 countdown and Ready text to new GUIText object instead of older GUI method.
- Added 3, 2, 1 countdown to start of level and after restart of current level.


## Alpha 2.0.1 - 2/8/15
- Player gains a life for completing a level.
- Limited width player can move.
- Limited player fire rate.
- Fixed bugs with syntax for mobile devices.
- Built first Android version.
- Added tilt steering for ship on Android devices. Turn device like a steering wheel.
- Added Level 3 with additional asteroid spawns.
- Tweaked game settings for difficulty level on Levels 1, 2, and 3.
- Added Enemy Turret for Level 3.
- Added additional asteroids to Level 3.
- Added turrets destroyed count to HUD starting on Level 3.
- Added total turrets destroyed to game over menu.
- Added engine particle FX.
- Added current level indicator to HUD.
- Added current level popup text when starting or restarting level.
- Added Go! text when starting level or restarting level.
- Added 3, 2, 1 countdown on restart level pause when player ship destroyed.
- Added skybox textures to backgrounds for more depth to the scene.


## Alpha 2.0.0 - 1/27/15
- Removed game menu background music ambient_menu.mp3.
- Added game main menu background music insert coin.
  - Credits: Insert Coin by megupets.
  - http://opengameart.org/content/insert-coin
- Moved main menu background music to game over music.
- Added Level2 for testing level transition logic.
- Added Debug.Log output for level transitions.
- Modified placement and fixed text ratios on gameplay screen.
- Added gameDifficulty variable to control gameDifficulty logic across levels.
- Added enemyRateOfFire variable to control enemyRateOfFire of fire logic across levels.
- Added gameSpeed variable to control overall gameSpeed logic across levels.
- Tweaked gameplay logic settings for Level 1 and Level 2.
- Added game menu background music Sci-Fi Close.
  - Credit: "Sky Game Menu" by Eric Matyas Soundimage.org
  - http://opengameart.org/content/sci-fi-close
- Total rewrite of enemy ship mechanics and enemy bullet mechanics.
- Redesigned game HUD layout.
- Updated main menu with image.
- Added Borderless Windowed Mode in Windows Setup program. (Check Windowed mode on config)
  - Add to any shortcut by adding -popupwindow to Target (On by Default on installer generated shortcuts).
- Added icon and associated graphics.

## Alpha 1.10.7 - 1/24/15
- Added logic to destroy all objects after they leave the game screen to reduce resource usage.
  - Needs testing.
- Added logic for basic enemy AI to track player.
- Added enemy ship weapon 1.
- Added ability for enemy ships to fire directly at player from any angle.
- Added customized enemy ship skin.
- Changed enemy ship model to actual models rather than different mesh to get better hit tracking.
- Tweaked point light to have better colors on enemy ships.
- Fixed menu links on main menu and game over menu.
- Added keyboard shortcuts for menu screens.
- Added a ton of comments to javascript files to help keep things in order.
- Added kill count to play screen.
- Added asteroids mined count to play screen.
- Added total kill count to game over menu.
- Added total asteroids mined count to game over menu.
- Added pause game functionality with keystroke esc or p while playing.
- Added Silkscreen font to game menu screens and game UI text.
  - Credit: Jason Kottke
  - http://www.kottke.org/plus/type/silkscreen/index.html
- Rearranged game UI text on gameplay screen for new fonts.


## Alpha 1.10.6 - 1/21/15
- Added asteroid obstacle and multiple asteroid spawners for testing. May reduce later for level 1.
- Added custom asteroid blender model using the add_mesh_rocks plugin.
- Added new model for player ship with customized skin.
- Added new model for enemy ship with customized skin.
- Tweaked many game mechanic values to compensate for asteroids.
- Added main menu link to game over menu. Can also press escape.
- Change text sizes and positions on game over menu to make room for additional menu items.
- Added ability to change amount of ships spawned, and additional spawners can be added.
  - This should lead to ability to spawn more enemies in harder levels.

## Alpha 1.10.5 - 1/19/15
- Added start screen.
- Added high scores page.
- Added credits page.
- Added main menu background music, Sky Game Menu.mp3.
  - Credit: "Sky Game Menu" by Eric Matyas Soundimage.org
  - http://opengameart.org/content/sky-game-menu
- Added Version # to start screen.
- Added deselect menu item sound. deselect01.ogg
  - Credit: K.L.Jonasson, Winnipeg, Canada. Triki Minut Interactive www.trikiminut.com
  - http://opengameart.org/content/sci-fi-selectdeselect-sfx
- Added player weapon 1 fire on left mouse click as well as spacebar.
- Added keystroke r to restart from game over menu.
- Added keystroke q to quit game from game over menu.
- Added keystroke f5 to take jpg screenshot.


## Alpha 1.10.4 - 1/19/15
- Added limited rate of fire of 3/second.
- Added a game timer with seconds counter. May use later for level up or other game mechanics.
- Added player ship laser sound effect, Laser2.wav.
  - Credit: 8-bit Platformer SFX commissioned by Mark McCorkle for OpenGameArt.org ( http://opengameart.org )
  - http://opengameart.org/content/8-bit-platformer-sfx
- Added explosion sound effect for ship explosions, Explosion.wav.
  - Credit: 8-bit Platformer SFX commissioned by Mark McCorkle for OpenGameArt.org ( http://opengameart.org )
  - http://opengameart.org/content/8-bit-platformer-sfx
- Added game menu mouseover sound effect, mouseover01.ogg.
  - Credit: K.L.Jonasson, Winnipeg, Canada. Triki Minut Interactive www.trikiminut.com
  - http://opengameart.org/content/sci-fi-mouseover-sfx
- Added game menu select sound effect, select01.ogg. 
  - Credit: K.L.Jonasson, Winnipeg, Canada. Triki Minut Interactive www.trikiminut.com
  - http://opengameart.org/content/sci-fi-selectdeselect-sfx
- Added final death sound effect, Retro_Game_Sounds_SFX_85.wav. 
  - Credit: Jesús Lastra.
  - http://opengameart.org/content/retro-game-sounds-sfx-volume-1
- Added take screenshot command, F5. Saved to Screenshots folder in game directory.

## Alpha 10.3 - 1/16/2015
- Added level 1 background music, circling.mp3. 
  - Credit: deadEarth
  - http://opengameart.org/content/circling
- Added game menu background music, ambient_menu.mp3. 
  - Credit: Alexandr Zhelanov
  - http://opengameart.org/content/ambientmenu
- Fixed game menu text being centered properly.

## Alpha 10.2 - 1/16/2015
- Trying to fix game menu being uncentered in build, but not in testing.

## Alpha 10.1 - 1/16/2015
- Switched to incremental version tracking.
- Reset score properly on game restart from game over menu.
- Added enemy ship explosion on collision with player ship.
- Added 100 point penalty for collision with enemy ships.
- Increased initial enemy ship speed to 13.

## Alpha 10 - 1/16/2015
- Added game restart functionality on game over menu.
- Added reset lives on game restart from game over menu.

## Alpha 9 - 1/16/2015
- Added game over menu with final score, restart game, and quit game menu items.
- Added quit game button functionality.
- Added arcade style scoring.
- Added 

## Alpha 8 - 01/15/2015
- Added lives(ships) tracking.
- Added reset of lives and score after 3 deaths.
- Modified projectile model to be more laser like.

## Alpha 7 - 01/15/2015
- Added score tracking.

## Alpha 6 - 01/14/2015
- Added colored textures to models.

## Alpha 5 - 01/14/2015
- Additional game mechanics tweaks.

## Alpha 4 - 01/14/2015
- Reduced size of player ship model.
- Added better hitboxes for enemy ship.

## Alpha 3 - 01/14/2015
- Added custom player ship model.

## Alpha 2 - 01/14/2015
- Additional game mechanics tweaks.
- Reduced size of enemy ship model.

## Alpha 1 - 01/14/2015
- Initial setup of game mechanics and physics.
- Added player controls for left and right.
- Added explosions.
- Added added shooting player projectiles.
- Added custom enemy ship model.
- Added collision of player ships, projectiles, and enemy ships.
- Added level restart on death.
- Added press escape to quit.
- Added projectile removal on hit.

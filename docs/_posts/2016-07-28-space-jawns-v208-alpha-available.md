---
date: 2015-04-08
title: Space Jawns v2.0.8 Alpha is available!
categories:
  - release
  - game news
author_staff_member: sk33lz
---

Once again it took a bit longer than I expected to take for a new release, but I ran into some snags with some of the features I planned to release in 2.0.8-alpha. I figure it's better to include more features in a release, so hopefully that's ok with everyone else.

There are a ton of new features and updates with this release, so I'm just going to let the Changlog do most of the talking. Highlights from this release include a new ship energy system, Levels 7-10, increased randomization, and more skyboxes!

Changlog
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

Check out the [Space Jawns download](/download) page to get the latest files.

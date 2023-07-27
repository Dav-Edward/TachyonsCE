# TachyonCE
Tachyon Community Edition

This is the community modified version of Tachyons: Battles Across the Galaxy. You can find the main game here:

https://spektor.itch.io/tachyon

Look for the official fully improved version coming to Steam here: https://store.steampowered.com/app/1350310/Tachyons_Battles_Across_the_Galaxy

Please note: This build of the game is now far behind the latest version of the game. Tachyons has integrated most of the features added of CE into the base game.
=======
![Tachyons CE latest version](https://img.shields.io/badge/dynamic/json.svg?label=Latest%20version:&url=https://api.github.com/repos/Dav-Edward/TachyonsCE/releases/latest&query=$.name&style=for-the-badge)

Build 1.0.2
Created Windows-Friendly launcher for the game and included JRE to make playing experience easier for Windows users.

Build 1.0.1.x
Added additional ship sprites courtesy of EditDotEXE.

Build 1.0.1
Updated subversion data to check client/server matching

Build 1.0

Tachyons CE release notes:

+Reverted Prison event changes due to breaking the event entirely. Kept only basic timer cleanups
+Fixed end game boss crashing the game in previous build

+Re-branded "Tachyon" to "Tachyons" to reflect the new name of the game and project
+Changed the main title splash screen
+Changed the main title music theme to a unique track made just for Tachyons CE by AlexBlackRaven
+Changed the game UI slightly to a blue theme instead of the green-teal original colour
+Changed game fonts to a nicer, easier to read font style that's easier on the eye
+Changed 'BreakOnUninstall' aka 'Rusty' non-weapon systems on ships. Now ships can be raided for everything on common ships. Most situations there is a 50% chance a system is 'rusty'
+Changed Engines, HyperDrive, and Shields in stores to reflect the fact players can steal inferior versions from common ships. The store versions are more upgradeable.
+Stopped D.F from wandering too far if the players are slow to catch up with it. (Currently limited to 9 jumps until the player spots it)
+Stopped trader ships spawning in hazard zones
+Optimized Prison events to use less timer events that fire less often to reduce server slow-down
+Fire is more dangerous
+Air depletes faster causing mobs to suffocate faster, but the damage taken from suffocation is slower
+Attempted to fix purchasing workers/slaves charging players multiple times if they own multiple ships

Commit ??-22:
+Lots of small changes
+Fixed missing EMP Cannon sprite from main campaign
+More minor dialogue fixes

Commit #11-14
+Added subversion support to detect server/client mismatches
+Minor spell fixes
+Minor main menu alteration

Commit #9
+Massive corrections to typos, spelling mistakes and general improvement to all dialogues in all sectors
Commit #10
+Minor changes to specific words for consistency such as HyperDrive and Hyper-Space

Commit #8
+Fixed StartServerConsole.sh to properly open TachyonServer.jar not just 'Tachyon.jar'
+Changed all existing dialogues to [SKIP][AUTO] to eliminate having to keep clicking ... to move conversations. If more than 6 happen in a row, a ... is left to stop the log scrolling too far
+Split a reply at the USC where the reply was so long a player's name would push it out of the dialogue screen. Now the NPC just replies with ... for the player to do two replies in a row
! Put an advisory in config.cfg that the server variable VEASION_PER_POWER although a typo cannot be corrected as that is what the actual variable is. Will change if a new JAR is compiled with that fixed later
+Deleted duplicate systems in the TUT folder that are absolutely identical to the Tutorial folder to prevent collisions and future issues
+Changed TP_LASER.sys to use IMAGE=LASER1-1 as it's almost identical other than the fact it breaks on uninstall
+Fixed a few typos in dialogues spotted while playing

+Added @Zone51's improved ship weapon assets to the project
+Changed Plasma Cutter weapon to use PLASMA.png base instead of BEAM.png Reverted change. Confused Plasma 'cutter/cannon/burst' with each other.
+Made the weapon 'Ejector' use its own unique weapon asset to not conflict with the new Railgun weapon assets
+Fixed Tutorial mission to look for the specific tutorial pirate ship instead of blindly count ships to avoid the game soft locking if players add additional ships to spawn before completing the tutorial
+Added EVENT function 'EJECT_ALL_CARGO' for ships and stations to call if you want to spit out all cargo
+Added EVENT function 'EJECT_CRYSTAL' for ships and stations to eject out the Hak86 crystal. It is not yet coded to trigger the event itself.
! Added a scratch pad file for developers to note code we might use in the project that doesn't yet have a home
! Added all noteworthy files from the client JAR file that we might want to edit. Do not change the folder structure as it's 1:1 with the original JAR

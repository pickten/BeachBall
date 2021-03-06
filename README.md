# BeachBall

Helper addon for Sandcastle Builder (http://castle.chirpingmustard.com/castle.html).

## Features

* Beach Autoclicking: Can be set to click the NewPix, just once per NP (to keep up Stealth/Ritual) or x times per second. Can be toggled between keeping Ninja Stealth or Ninja Ritual.
* Kitties: Kitties have a timer on top of the screen, to tell you when there is a kitty. Can be set to autoclick kitties, or to auto-focus on the kitty.
* Logicats: Can be set to solve automatically. Caged logicats can automated, solving one by one, the maximum at once for QQ, or to get bonemeal.
* Monty Haul: Can be set to auto-puchase and solve, either attempting for the 'prize' or the goat.
* Temporal Rifts: Can be set to use automatically use rifts, either to farm flux crystals or for the ONG.
* Tool Factory: The TF can be loaded faster (does not require TF Load Letter).
* Faves Autoclicker: Using the Faves panel, any boost can be set up with an autoclick timer. (An example use would be to autoclick Question Qubes.)

(Audio alerts are currently non-functional.)

## How to use this script ?

Start by installing this script (http://github.com/codeRitter/BeachBall) using one of two methods:

A. If you have Greasemonkey (for Firefox) or Tampermonkey (for Chrome), install BeachBall_Monkey_Loader.js (instuctions for using Xmonkey can be found elsewhere). The BeachBall addon will automatically load 5 seconds after loading the game page (you must reload the game page once after installing - don't forget to save).

B. If you do NOT have one of those addons, copy the contents of BeachBall_Bookmark_Loader.js into a bookmark (paste onto the link/location/destination, and not the description or name). You will need to click your bookmark once to get the BeachBall addon to load - EVERY time you reload the game page, you must reclick the bookmark loader.

Once loaded, go in the Option panel of the game, and you will find every option to enable at the bottom of the panel.

####Special Feature: Faves Autoclicker
This feature is performed using the Faves panel instead of the Options panel.
* To set an autoclicker for a boost, open the Faves panel and select the desired boost (if the boost is not already in the dropdown selection, use the 'Choose' button to make a new fave). With the boost selection, click 'AutoClick' and follow the directions on the popup to set the timer. The timer frequency can be changed later using the same process.
* To disable (or view) a Faves autoclicker, select the boost in the Faves panel and toggle 'Visible' on. On the visible Fave boost, there should be a timer adjacent to the category label (looks like '[ 1s ]'). Click this timer to disable the boost autoclicker.

## Changelog

###Version 5.3.1.1

####Bug Fixes
* No longer unintentionally clicking 1/NP if Ninja Mode:Ritual and Beach Autoclicker:Off.
* Fixed highly unlikely edge case if you constantly spawn Temporal Rifts (via tons of single Logicats, for example) in Ninja Ritual with Autoclicker on, where you could miss extending the ritual and then possibly click for stealth.

###Version 5.3.1

####Changes
* Ninja Ritual has been split from Beach AutoClick. Beach Autoclick has only 3 modes again: Off, Click once per NP, CPS. There is a new option: NPB Ninja Mode, which can be set to either Ninja Stealth or Ninja Ritual. Now you can toggle your autoclicker when the NPB timer is counting down! Players who previously used CPS (ritual) will have their mode initially set to Ritual, everyone else will be initally set to Stealth. (As a side note, this change means you should be able to ritual without clicking once a second and without Herder.)
* Refresh Rate is now changable. Set it lower to have BeachBall execute commands (such as kitties) faster, or set it higher to slow the addon down.

###Version 5.3.0

####Changes
* Audio (which didn't work) has been removed.

####Fixes
* ONG Rift logic (to account for Aleph One and cracks).
* 'Cristal' is no longer a word.

###Version 5.2.0.5

####New Features
* Flux Harvest will now be used to harvest flux if it is available.
* NEW: Clear log option. Clears the in-game log to reduce lag.

####Bug Fixes/Improvements
* Improvements to logicat, including max solve fix.

###Version 5.2.0

####Features
* NEW : Favorite autoclick - In the Favorite pannel, you can now assign an autoclick to any set favorite. Doing so will ask you for a timer, and may ask you to choose a button to click if there are multiples. If you proceed so, you will have a timer that you can click for activating and de-activating the timer. You can remove it completely by starting assignation of a new timer and canceling it. This can be used to trigger Question Qubes over time, or improving sand industry regularly after a molping down, reducing repetitive spaming activities in just a few clicks.
* Improving Beach Autoclick by adding an "ninja ritual" setting, that will ninja every NP, gathering goats.
* NEW : Rift Autoclick - 2 settings. "Gather Flux Cristals" will use rifts after they close until you have no more Time Lord rift available, and waiting for the NPB to have been ninja'd. "ONG" will use rifts to create a maximum of ONGs. It will always wait for the game to have sand (for building from blackprints) and will wait for the NPB to have been ninjad.



###Version 5.1.4.0 - .2

####Bug Fixes
* Fixed Logicat countdown and clicker not working with Redacted object rewrited in 3.33331
* Fixed option menu rewriten in same update
* .1 : Fixed Logicat bug with audio alert
* .2 : Fixed display problem with classic layout

###Version 5.1.3

####Bug Fixes
* Fixed Logicat solver to work with latest SCB changes.

###Version 5.1.2

####Bug Fixes
* Fixed Logicat solver to work with latest SCB changes.

###Version 5.1.1

####New Features
* Re-implementing Pure Logicat Solver

###Version 5.1

####New Features
* Logicats in a redundakitty chain are being solved.
* Caged AutoClicker can solve single puzzles (1 per 5 seconds)
* Caged AutoClicker can solve maximum puzzles (using this setting without having ZooKeeper may cause problems)
* Caged AutoClicker can trade 100+ logicats for bonemeal (must have Shadow Dragon unlocked)

###Version 5.0

####New Features
* Caged Logicat Autosolver implemented as Full Auto and re-enabled.

####Temporary Bug Fixes/Workarounds
* Logicats in a redundakitty chain are still set to auto-hide.

###Version 4.9.9

####Temporary Bug Fixes/Workarounds
* Due to massive changes in v3.292 of Sandcastle builder, several features have been disabled in this build to allow it to function until a proper patch can be issued.
* Caged Logicat AutoSolver has been Disabled
* LC Solver will now Auto-Hide Logicats if they spawn.

####Bug Fixes
* LC audio alert fixed.

###Version 4.2

####Bug Fixes
* With high logicat/AC, temporal rift is essentially permanent, preventing Keep Ninja AutoClick from processing. Caged Logicat Autoclicker will now pause to process the click (allow Temporal Rift to expire), then resume.

###Version 4.1

#### New Features
* Can now choose whether you want Monty Haul Problem AutoClicker to try and find a Goat or a Prize (and works with Beret Guy if unlocked).

####Bug Fixes
* Updated list of Redundakitty locations.

###Version 4.0.4

####Bug Fixes
* Fixed Caged Logicat Autoclicker.
* Fixed Tool Factory helper.

###Version 4.0.3

####Bug Fixes
* Removed some debugging notifications that were accidentally left in.

###Version 4.0.2

####Bug Fixes
* Caged Logicat solver is really fully working this time!

###Version 4.0.1

####Bug Fixes
* Caged Logicat solver working again with latest SCB version (v 3.261)

### Version 4.0

#### New Features
* Caged Logicat AutoClicker now implemented
* Monty Haul Problem AutoClicker: AutoBuy if available and Opens Door(s)
* Settings are now saved between sessions if HTML5 local storage is available.

#### Feature Changes
* Simplified AutoClicker and Logicat solver options.
* Redundakitty AutoClicker will no longer open menus to click them (unless the Find RK option is enabled).
* Beach AutoClicker works better (clicks evenly over time, rather than in a large clump every tick).

### Version 3.4.1

#### Bug Fixes
* Fixed to work for people who have not yet unlocked Tool Factory.

### Version 3.4

#### New Features
* Tool Factory option to load a user defined amount of glass chips into the tool factory. Click on the number of chips to change. Click Load Tool Factory to load chips.

#### Bug Fixes
* Removed Border Alerts as this is provided by the Beach Ball boost in game.
* Fixed RedundaKitty and LogiCat AutoClick to work with new layout.
* Changed the LogicCat option item name to more accurately reflect its current ability as it does not AutoClick LC's/Caged LCs, just solves them if available.

### Version 3.3

#### Bug Fixes
* Redundakitty autoclicker will now work when the redundakitty spawns in the Discoveries and Momuments/Glass Monuments tabs.
* Discovery and Monuments menus should now toggle correctly when RK Finder/AutoClicker is enabled.

### Version 3.2

#### Bug Fixes
* Fixed syntax in Bookmark loader (missing semi-colon).
* Fixed minor error in setting auto click CPS change rate dialogue.
* Fixed Beach Auto Click so it should keep going after ninja stealth streak.

### Version 3.1

#### Bug Fixes
* Beach autoclicker will no longer break ninja streak.

###Version 3.0

#### New Features
* Caged Logicat solver implemented (under the Logicat Auto Clicker option).
* Logicat only audio alert implemented.
* Beach Auto Clicker Implemented. Options are "Off", "Keep Ninja" (to only click once per ONG to maintain Ninja streak), and "On" with clicking rate from 1 to 20 CPS (clicks per second).

#### Bug Fixes
* Fixed ONG only audio alert so it actually works.

#### Behind the Scenes
* Namespaced variables/methods in a BeachBall object to prevent potential JS crossover issues. It's not pretty, but I think it works.

### Version 2.1

#### Bug Fixes
* RedundaKitty autoclicker should now properly deal with YouTube RedundaKitties
* RedundaKitty autoclicker should now properly deal with Redundant RedundaKitties
* Ninja streak autoclicker shouldn't click during a temporal rift.

### Version 2.0

#### New Features
* Menu system implemented
* Ninja streak autoclicker implemented
* RedundaKitty finder and autoclicker
* Logicat solver/autoclicker
* Ninja streak visual cues
* Redundakitty audio alerts

===

### Version 1.0
*My really rough first attempts at coding an add-on.

# Star Wars Jedi Knight: Jedi Academy - nettux433's mod

## Install

Download the latest release and extract the contents of this zip into your GameData/ folder

## Changes

 * Team FFA saber colours for blue team may now be anything but red
    (instead of only blue)
 * Power Duel is now a duel between 2 teams totaling up to 12 players
   - Change g_nettuxPowerDuelBotTeam to choose bot team assignment behaviour
      (0 => balance, 1 => lone, 2 => double)
   - All players on both teams should always start with 100hp
   - Player wins are given if you're team wins AND you survive the round
   - Player losses are given if you die AND your team loses
 * Add Regen option
  - g_nettuxRegen set to 1 will enable regeneration, 0 will disable it
  - g_nettuxRegenTimer is the number of seconds that must pass without
    taking damage before regeneration begins
  - g_nettuxRegenInterval is how many seconds between player health increments
  - g_nettuxRegenAmount is how much regeneration increments player health by
  
## For players

To install OpenJK, you will first need Jedi Academy installed. If you don't already own the game you can buy it from online stores such as [Steam](http://store.steampowered.com/app/6020/), [Amazon](http://www.amazon.com/Star-Wars-Jedi-Knight-Academy-Pc/dp/B0000A2MCN) or [GOG](https://www.gog.com/game/star_wars_jedi_knight_jedi_academy).

Installing and running OpenJK:

1. [Download the latest build](http://builds.openjk.org) for your operating system.
2. Extract the contents of the file into the Jedi Academy `GameData/` folder. For Steam users, this will be in `<Steam Folder>/steamapps/common/Jedi Academy/GameData`.
3. Run `openjk.x86.exe` (Windows), `openjk.i386` (Linux 32-bit), `openjk.x86_64` (Linux 64-bit) or the `OpenJK` application (OS X), depending on your operating system.
 
**Linux Instructions**

If you do not have a windows partition and need to download the game base.

1. Download  and Install SteamCMD [SteamCMD](https://developer.valvesoftware.com/wiki/SteamCMD#Linux) .
2. Set the download path using steamCMD, force_install_dir <path> .
3. Using SteamCMD Set the platform to windows to download any windows game on steam. @sSteamCmdForcePlatformType "windows"
4. Using SteamCMD download the game,  app_update 6020.
5. [Download the latest build](http://builds.openjk.org) for your operating system.
6. Extract the contents of the file into the Jedi Academy `GameData/` folder. For Steam users, this will be in `<Steam Folder>/steamapps/common/Jedi Academy/GameData`.


**OS X Instructions**

If you have the Mac App Store Version of Jedi Academy, follow these steps to get OpenJK runnning under OS X:  

1. Install [Homebrew](http://brew.sh/) if you don't have it.
2. Open the Terminal app, and enter the command `brew install sdl2`.
3. Extract the contents of the OpenJK DMG ([Download the latest build](http://builds.openjk.org)) into the game directory `/Applications/Star Wars Jedi Knight: Jedi Academy.app/Contents/`
4. Run `openJK.app` or `openJK SP.app` 
5. Savegames, Config Files and Log Files are stored in `/Users/<USER>/Library/Application Support/OpenJK/`


## For Developers

### Building OpenJK
* [Compilation guide](https://github.com/JACoders/OpenJK/wiki/Compilation-guide)
* [Debugging guide](https://github.com/JACoders/OpenJK/wiki/Debugging)

### Contributing to OpenJK
* [Fork](https://github.com/JACoders/OpenJK/fork) the project on GitHub
* Create a new branch and make your changes
* Send a [pull request](https://help.github.com/articles/creating-a-pull-request) to upstream (JACoders/OpenJK)

### Using OpenJK as a base for a new mod
* [Fork](https://github.com/JACoders/OpenJK/fork) the project on GitHub
* Change the GAMEVERSION define in codemp/game/g_local.h from "OpenJK" to your project name
* If you make a nice change, please consider back-porting to upstream via pull request as described above. This is so everyone benefits without having to reinvent the wheel for every project.

### Deciphering buildbot's output
* Pick the build from the operating system builder you're interested in at the [builders](https://jk.xd.cm/builders) page.
* Click on stdio for the Steps to see the command executed and the result.
* The command is at the very top, the output starts below.

## Maintainers (in alphabetical order)

* Ensiform
* Razish
* Xycaleth

## Significant contributors (in alphabetical order)

* eezstreet
* exidl
* ImperatorPrime
* mrwonko
* redsaurus
* Scooper
* Sil
* smcv

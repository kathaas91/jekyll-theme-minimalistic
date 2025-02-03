# How To Mod Skyrim SE Manually

The Elder Scrolls V: Skyrim is an open-world RPG developed by Bethesda Game Studios and released in 2011. It has received several ports and upgrades over the years. For the purposes of this guide we will be using the "Special Edition" from the Steam store.

While it is easier and recommended to mod Skyrim using a mod organizer (such as MO2) it is not necessary to do so, especially if installing few or simple mods. The requirements and set up to prepare Skyrim to be modded are the same regardless of if modding the game manually or using additional software.

## Tools  
For this guide you will need:

* [A copy of Skyrim SE from Steam](https://store.steampowered.com/app/489830/The_Elder_Scrolls_V_Skyrim_Special_Edition/)
* [A free Nexus Mods account](https://www.nexusmods.com/)
* [SKSE64](https://skse.silverlock.org/)

## Preparing Skyrim  
You will need a clean install of Skyrim SE. If you already have Skyrim installed on your computer, uninstall it from your Steam library then delete any remaining files in the steamapps->common folder and Documents->My Games.

To set up Skyrim to be modded, follow these steps:
1. Reinstall Skyrim from your Steam library
2. Launch the game via Steam
3. Choose your preferred options from the launcher; this will determine the settings generated in the Skyrim.ini and SkyrimPrefs.ini
4. Click “Play” and launch the game
5. Once the main menu has loaded, exit back to your desktop.

## Installing SKSE64
Skyrim Script Extender (SKSE64) is an essential utility for many mods that increases the functionality of Skyrim's game engine. It is important to check what version of Skyrim SE you installed and download the appropriate SKSE64 build.

Open the downloaded zip folder and extract all of the files inside the skse64 folder into Skyrim's root folder (the folder where Skyrim's excecutables are located). Overwrite any existing files when prompted.

## Downloading Mods From Nexus Manually 
For the purpose of this guide we will be installing SkyUI. SkyUI is the most endorsed mod of all time for Skyrim SE and is also a requirement for many other mods to function properly.

[SkyUI Nexus Mods Page](https://www.nexusmods.com/skyrimspecialedition/mods/12604)

It is important to read the “Description” page for any mod you are installing, as it not only contains a description of what the mod is and does but also important information about version requirements and compatibility with other mods.

1. Click on the “Files” tab. SkyUI only has one file, but many mods have several. You will usually only need the most recent file under “Main Files.”
2. Click “Manual Download.”
3. The mod will now start to download to the default location for your browser or a location of your choice.

## Installing SkyUI 
For the majority of mods most or all of the mod files will go into the "Data" folder in Skyrim's root folder. This is where all of the various data files for the game and its expansions are kept.
1. Once the download is done, open or extract the zip file containing the mod files.
2. Copy all files from the mod folder and paste them in the Skyrim SE -> Data folder. Overwrite if necessary.

## Activating Mods
When manually modding Skyrim it is required to also manually activate or deactivate any installed mod files located in the "Data" folder via the Skyrim launcher.
1. Launch the Skryim SE Launcher through Steam.
2. Select "Data Files."
3. Tick the box for "SkyUI_SE.esp."
4. Apply and close the window and exist the launcher.

## Launching Modded Skyrim
SkyUI and many other mods require SKSE to load properly. This means that Skyrim needs to be run through the skse64.exe file installed earlier in this guide. While it can be run by navigating to the game folder every time you want to play the game, it is easier to either create a desktop shortcut or re-direct Steam to launch the game through SKSE instead of the launcher.

### Creating a desktop shortcut for SKSE
This method will automatically generate a shortcut to skse.exe on the desktop that can be used to launch the game.
1. Navigate to Skyrim's root folder and right-click on skse64.exe
2. Click "Show more options"
3. Click "Send to" and choose "Desktop (create shortcut)."

### Launching SKSE through Steam
This method will change the path that Steam uses when looking for the game excecuteable, letting you continue to launch the game directly through Steam.
1. Right click on Skyrim in your Steam library.
2. Click on "Properties"
3. Click on "Set Launch Options..."
4. Enter the file path for skse64.exe in quotes followed by %command%.
For example: `"C:\Program Files (x86)\Steam\steamapps\common\SkyrimSpecialEdition\skse64.exe" %command%`

You have now successfully modded Skyrim SE! Enjoy your adventures!

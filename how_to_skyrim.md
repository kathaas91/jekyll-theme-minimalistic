# How To Install Skyrim SE Mods With MO2  
The Elder Scrolls V: Skyrim is an open-world RPG developed by Bethesda Game Studios and released in 2011. It has received several ports and upgrades over the years. For the purposes of this guide we will be using the "Special Edition" from the Steam store.  

Mod Organizer 2 is a popular modding utility that makes downloading, installing and managing mods simple by creating installation instances separate from the base game files and providing built-in tools and utilities to ensure modded games run smoothly.

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
Skyrim Script Extender (SKSE64) is an essential utility for many mods that increases the functionality of Skyrim's game engine. It is important to check what version of Skyrim SE you installed and download the appropriate  build.

Open the downloaded zip folder and extract all of the files inside the  folder into Skyrim's root folder (the folder where Skyrim's excecutables are located). Overwrite any existing files when prompted. The root folder should look like this:

![image](https://github.com/user-attachments/assets/69d9a597-c026-495d-9942-90d73d5edb89)


## Installing MO2  
MO2 can be installed from it's official [Nexus Mods](https://www.nexusmods.com/skyrimspecialedition/mods/6194?tab=description) page or its [GitHub repository](https://github.com/Modorganizer2/modorganizer/releases). Download the main file from either source and run the downloaded .exe file. It is recommended to install MO2 outside the C: drive, or in a separate dedicated folder on the C: drive, for example C:\Modding\MO2.

1. Upon launching MO2, you will be prompted to create a new instance. Choose “Create a portable instance.” This will store everything in MO2's installation folder. Click “Next.”
2. You will then be prompted to select what game you want to manage. Skyrim should auto-populate but if it does not you can select “Browse” and manually navigate to the folder the Skyrim.exe and SkyrimLauncher.exe are located in. Click “Next.” Select the game edition, in this case, Steam.
3. On the next screen, “Automatic archive invalidation” will be checked by default. It is also recommended to choose to use profile-specific saves and INI files to make it easier to test and switch between different mod setups. Click “Next.”
4. Now you will select where to store the data for MO2 for your new instance. The default location is fine and does not need to be changed unless there is a specific reason. Click “Next.”
5. Confirm your settings are correct and click “Finish.”
6. When MO2 launches your new instance for the first time you will be asked how you want to handle the default category setup. Either option is fine.

![image](https://github.com/user-attachments/assets/67a1c0eb-b0e1-4679-a0d0-f75dde39bff8) ![image](https://github.com/user-attachments/assets/7d405b46-5a9b-4348-ada4-fe4154f740aa)
![image](https://github.com/user-attachments/assets/4b3fabb3-1d84-4a4f-b226-0cb3d0accf49) ![image](https://github.com/user-attachments/assets/42c78097-e4d1-454f-b378-c5db34ed72a0)
![image](https://github.com/user-attachments/assets/3c4b2209-f1f9-43aa-b5f6-3c4d395c655c) ![image](https://github.com/user-attachments/assets/2d2ce43e-c0ee-451f-8bf5-46000a092bc0)

### Linking MO2 to Nexus Mods  
You are now on the MO2 home screen! The first thing we need to do here is link MO2 to your Nexus Mods account and associate NMM links with it.

1. On the top menu, click the icon on the far right. This will open the settings menu.
2. Click the tab that says Nexus, then “Connect to Nexus.” This will open a new browser window or tab.
3. If you are not already logged in, you will be prompted to enter your username and password. Click “Authorize.” 
4. In MO2 click “Associate with “Download with manager” links and if prompted click “Yes.” This will ensure that when choosing to download mods from Nexus with a mod manager that they will be downloaded through MO2. 
5. Restart MO2 if prompted and click “Yes” to set up MO2 to handle nxm links.

![image](https://github.com/user-attachments/assets/57138a48-bdab-492e-b81a-2c77801a757a)
![image](https://github.com/user-attachments/assets/2f61e580-c8db-4703-8f61-956bc4eb8398)

You are now ready to start downloading mods!

## Downloading Mods From Nexus With MO2  
For the purpose of this guide we will be installing SkyUI. SkyUI is the most endorsed mod of all time for Skyrim SE and is also a requirement for many other mods to function properly.

[SkyUI Nexus Mods Page](https://www.nexusmods.com/skyrimspecialedition/mods/12604)

It is important to read the “Description” page for any mod you are installing, as it not only contains a description of what the mod is and does but also important information about version requirements and compatibility with other mods.

1. Click on the “Files” tab. SkyUI only has one file, but many mods have several. You will usually only need the most recent file under “Main Files.”
2. Click “Mod Manager Download.”
3. The mod will now start to download through MO2. You can click on the “Downloads” tab on the right hand window to see the progress.

![image](https://github.com/user-attachments/assets/e1752cd0-bf91-4da3-804c-07b618f4a138)

### Installing and Activating Mods With MO2  
Once the download is done, double click on the mod file name. You can ignore any pop-ups about categories by clicking "Proceed." For some mods, like SkyUI, this will just extract and properly install the mod files. For others, it will open a separate installer.

To activate SkyUI, click the checkbox next to it on the left-hand panel.

![image](https://github.com/user-attachments/assets/c785c1b1-ea25-482d-9f93-0b2453f1a116)

## Running Modded Skyrim Through MO2
SKSE will likely be automatically added as an excecuteable by MO2 when it detects the exe file, but if it does not, it will need to be added. On the upper right hand side of MO2 is a dropdown box with links to all the excecutable files in the game's root folder as well as options to run the game and create a shortcut. In order for SkyUI to work properly, Skyrim needs to be run through the SKSE64 exe file.

1. Click on the dropdown box and click “Edit” at the very top. This menu shows the details for every exe file in this instance.
2. Click the + button above the excecutables list.
3. Click “Add from file.”
4. Navigate to the Skyrim SE root folder and select skse64_loader.exe.
5. Change the title of the exe if you wish, then click “Apply” then “OK.”
6. SKSE64 has now been added to the dropdown box.
7. Select SKSE64 then click “Run.”
8. The game will now boot up via the script extender with SkyUI running.
9. It is recommended to add a shortcut to this exe to easily launch the MO2 instance.

![image](https://github.com/user-attachments/assets/bb192417-7c1a-463c-887c-07f05033b228)


You have now successfully modded Skyrim SE! Enjoy your adventures!

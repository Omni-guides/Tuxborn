![Tuxborn Banner](https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/Tuxborn/Tuxborn_Banner.png)

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/D1D8H8WBD)


 ---


## Full Tuxborn Install Guide (SteamDeck)

If you have enough disk space available on your Steam Deck, you can now carry out the entire download and installation of Tuxborn via Wabbajack entirely on the Steam Deck. The total space required for this would be ~337GB, though this is made up of both the Installation and the downloads (which can be deleted once the install is complete).

If you do not have enough disk space available, then you will need to run Wabbajack on another system, and then transfer the Installation directory from that other system, to your Steam Deck. You can see details on transferring from a Windows system to the Steam Deck <HERE>, and resume this guide from Step 3.

If Wabbajack is new to you, or you haven't tried to run a Wabbajack Modlist on the deck before, the below process may seem very complicated and a daunting process. Not going to lie, it isn't the easiest thing to do in life, but it is very rewarding once complete!

It is **STRONGLY RECOMMENDED** to have Nexus Premium for the install process.

The following should be carried out in Desktop mode.

There are two parts to getting Tuxborn running on Steam Deck - Firstly the Wabbajack application, which will download and install the modlist, and secondly the post-install requirements. I have done my best to automate as much as I can of both parts (yes, doing this all manually would be _even longer_!)

You will need to have Skyrim Special Edition Installed on your Deck, and have started it once to main menu, and allow it to download all the CC Content when prompted.


---


### STEP 1 - Install Wabbajack via Steam/Proton

#### 1.1 - Create a Wabbajack Directory and Download Wabbajack

There are only a couple of steps that I can't automate for this - Downloading the Wabbajack installer, adding it to Steam, and running the initial launch.

While not specifically required, I strongly recommend you create a directory to use for Wabbajack, just to keep things in a sensible place and together. You can use a file browser or cli to create this new directory - for this guide I will use /home/deck/Wabbajack, but the commands shown will use the $HOME variable, which should apply the command to your user home directory on your system.

```
mkdir -p $HOME/Wabbajack
```

Next, download the Wabbajack Application into the Wabbajack directory we created:

```
wget -O $HOME/Wabbajack/Wabbajack.exe https://github.com/wabbajack-tools/wabbajack/releases/latest/download/Wabbajack.exe
```

Alternatively, just download it from [https://www.wabbajack.org/](wabbajack.org) via your browser and then copy or move it into the new Wabbajack directory. Either way, once you have a $HOME/Wabbajack/Wabbajack.exe in place, we're good to proceed.


#### 1.2 - Add Wabbajack.exe to Steam

Add Wabbajack.exe to Steam by using the "Add a Non-Steam Game to My Library" function from Steam:

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/shared/Shared-AddNonSteamGame.png" width="600">

In the window that appears, click the "Browse" button at the bottom:

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/shared/Shared-AddNonSteamGameBrowse.png" width="600">

Browses to the path of your Wabbajack.exe, which if you are following these instructions exactly, will be /home/deck/Wabbajack/Wabbajack.exe:

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/shared/Shared-AddNonSteamGameWabbajack.exe.png" width="600">

Click "Add Selected Programs":

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/shared/Shared-AddNonSteamGameAddSelectedProgram.png" width="600">

Once added, right click the new Wabbajack.exe entry in steam, and go to Properties. You can change the name to simply "Wabbajack" if you wish:

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/WabbajackProton/WabbajackProton_SteamProperties.png" width="600">

Next, click the Compatibility tab, and set it to use "Proton Experimental":

<<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/WabbajackProton/WabbajackProton_SteamCompatibility.png" width="600">

With that set, close the properties window and click Play for the Wabbajack entry in Steam. This will start Wabbajack for the first time, which is when the application downloads and installs the latest version of Wabbajack for you. It'll take a little time to download and install, just let it complete.

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/WabbajackProton/WabbajackProton_WabbajackInstalling.png" width="600">

Once done, the Wabbajack application itself should open up - **Close it down** before trying to use the application, and move on to Step 4.


#### 1.3 - Run the WabbajackProton Install script

I've written a bash script [(source)](https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/binaries/WabbajackProton.sh) that will configure the Proton Prefix as required to run Wabbajack via Proton. Run the following in a terminal/konsole and follow the few steps when prompted:

```
bash <(curl -s https://raw.githubusercontent.com/Omni-guides/Wabbajack-Modlist-Linux/refs/heads/main/binaries/WabbajackProton.sh)
```

e.g:

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/WabbajackProton/WabbajackProton_RunWabbajackProton.sh.png" width="600">


---


### STEP 2 - Run Wabbajack

#### 2.1 Nexusmods Login

All being well, that should really be all that is needed. Start Wabbajack from Steam again, and log in to Nexus using the little cog in the top right, followed by the Login button:

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/TuxbornFull/WabbajackProton_NexusLogin.png" width="600">

#### 2.2 Install from Disk (Once Tuxborn is available from the Wabbajack Gallery, this will be updated)

Until Tuxborn becomes available directly from the Wabbajack Modlist Gallery, you will need to manually download the Wabbajack file from here: [Tuxborn Nexus Mods](https://www.nexusmods.com/Core/Libs/Common/Widgets/DownloadPopUp?id=540642&game_id=1704). This will download a .zip file, and you will need to extract the Tuxborn.wabbajack file from inside the zip file. This will be far easier once Tuxborn is on the Wabbajack Gallery, which should happen soon!

Back in Wabbajack, once the Nexus Login is done, use the "back" arrow in the top left to return to the main Wabbajack menu, and click "Install from disk":

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/TuxbornFull/WabbajackProton_InstallFromDisk.png" width="600">

Click the three dots next to the "Target Modlist" line. A file browser window should appear - use it browse to the extracted Tuxborn.wabbajack file (NOTE. *Not* the .zip file, you must unzip this to access the Tuxborn.wabbajack file). Fill in the Install and Downloads directories using their Z:\ paths. I recommend following the paths below:

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/WabbajackProton/WabbajackProton_WabbajackInstallPaths.png" width="600">

This will keep the Install directory and Downloads directory separate, which will be a benefit in future as the Downloads directory can be deleted once things are all up and running correctly, to free up some space.

#### 2.3 Additional Notes

If you have attempted to install Tuxborn before, or you are updating it, you will need to tick the "Overwrite" box. When running Wabbajack via Proton, this doesn't show up very well, but you should be able to briefly see a tick in the box when you click it.

There are a couple of larger mods that sometimes fail to download when using Wabbajack in this way. You can avoid issues by manually downloading these mods and placing them into your Wabbajack Downloads directory that you set above

 - [Cleaned Skyrim SE Textures](https://www.nexusmods.com/skyrimspecialedition/mods/38775?tab=files&file_id=497442) - (Filename: 1_Kart_CSSET_POST_1.6.1130-38775-1-2-3-4-1714757549.7z)

#### 2.4 Start the Wabbajack Install

Once you are ready, click the Play button and the Wabbajack application should start to download all the mods needed for Tuxborn. This will likely take quite a long time - the downloads phase of the process is entirely dependant on your internet connection speed. As above, Nexus Premium is **strongly recommended**.

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/WabbajackProton/WabbajackProton_WabbajackClickPlay.png" width="600">

As a reminder, running Wabbajack on Linux/SteamOS is not a supported method, but we've done what we can to make things work as smoothly as they can. You may encounter crashes, or hanging - if this happens you can just restart Wabbajack, Click Install from disk, and click Play again - it should have re-populated your previous paths etc. It also may appear to have hung, but hasn't - This is especially true during the Building BSA's part of the Wabbjack process - please be extra patient here as it takes **a vary log time** on the Steam Deck hardware (See [Additional Notes](https://github.com/Omni-guides/Tuxborn/blob/main/TuxbornSteamDeckFullInstall.md#additionals-notes) for some indication of install times on Steam Deck.)

### STEP 3 - Post-Wabbajack Steps

Unlike on Windows, the Wabbajack Installation process is only part of what is needed on SteamDeck/Linux. There are a number of post-install steps that need to be carried out before the modlist is playable. Again, I've done my best to automate this, but there are still a few steps that must be done manually.

#### 3.1 Add Tuxborn's ModOrganizer.exe to Steam

Click the "Add a Non-Steam Game to My Library" option from the Games menu in Steam:

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/WabbajackProton/WabbajackProton_AddNonSteamGame.png" width="600">

Click Browse:

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/WabbajackProton/WabbajackProton_BrowseNonSteamGame.png" width="600">

and browse to the path for Tuxborn, which if you are following my recommendations, should be `/home/deck/Games/Skyrim/Tuxborn`

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/WabbajackProton/WabbajackProton_BrowseToMO2.exe.png" width="600">

Lastly for this step, click "Add Selected Program"

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/WabbajackProton/WabbajackProton_AddSelectedProgram.png" width="600">

#### 3.2 Properties of Tuxborn Steam Entry

When you add ModOrganizer.exe to Steam, it will be added with the name "modorganizer.exe" which is both not very helpful, and also won't be detected by my post-install automation script. Right click the "modorganizer.exe" entry, and click properties:

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/WabbajackProton/WabbajackProton_AddNonSteamPropertiesClick.png" width="600">

In the properties window, give it a more sensible name, I recommend "Skyrim - Tuxborn" - the "Skyrim - " part is particularly important to allow my Script to detect things correctly, so please just go with my recommendation unless you know what you are doing.

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/WabbajackProton/WabbajackProton_AddNonSteamProperties.png" width="600">

Switch to the Compatibility tab, tick the box for "Force the use of a specific Steam Play compatibility tool", and select "Proton Experimental":

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/WabbajackProton/WabbajackProton_AddNonSteamPropertiesCompatibility.png" width="600">

#### 3.3 Run once and reboot

To create the Proton Prefix and register Tuxborn with Steam so that this all works, you need to click Play on your Tuxborn entry in Steam, and **whether it loads Mod Organizer 2 successfully or not**, you _must close it down and move on to the next steps_, it will not work if you jump ahead and try to play the game at this stage.

#### 3.4 Automated Install Script

To run the required post-install steps automatically, you can run my automation script directly from GitHub [https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/binaries/omni-guides.sh](source) by pasting the following command in a konsole window and following the on-screen instructions:

`bash <(curl -s https://raw.githubusercontent.com/Omni-guides/Wabbajack-Modlist-Linux/main/binaries/omni-guides.sh)`

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/omni-guides.sh/Omni-Guides-sh_RunScript.png" width="600">

A banner and a short note will be displayed, and a request to press any key to continue:

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/omni-guides.sh/Omni-Guides-sh_BannerContinue.png" width="600">

The script will then attempt to detect any Wabbajack Modlists you have installed and added to Steam - in this case, Tuxborn. Type the corresponding number next to Tuxborn (e.g. 1) and hit enter:

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/omni-guides.sh/Omni-Guides-sh_SelectModlist.png" width="600">

You will be asked to confirm you want to continue, and the script will move on to detecting the Modlist Install directory - if you are using my recommended directory names and paths, this should be detected automatically. However, if you have called the directory something else, or if multiple possibile directories are found, you'll be asked to select the right one. If nothing can be found automatically, you'll be asked to manually input the path to the Modlist directory.

You will be prompted for your *sudo* password so that various permissions can be set correctly, and the script will continue through more automated tasks:

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/omni-guides.sh/Omni-Guides-sh_SudoPassword.png" width="600">

Lastly, you will be asked if you want to set the resolution. This is optional but I'm trying to reduce the manual steps as much as I can. If you're running this on a Steam Deck, it will assume the desired resolution is 1280x800 (If you are going to be playing while docked, you will have to manually alter the resolution via MO2 in the "Tuxborn - Settings" -> INI Files -> SSEDisplayTweaks.ini file. See [Additional Notes](https://github.com/Omni-guides/Tuxborn/blob/main/TuxbornSteamDeckFullInstall.md#additionals-notes) below for more information). If you are not running this script on a Steam Deck, you will be asked to input your desired resolution, in the format 1920x1080.

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/omni-guides.sh/Omni-Guides-sh_SetResolution.png" width="600">

#### 3.5 With the post-install automation script complete, you now need to REBOOT YOUR STEAM DECK, and then switch back to Desktop Mode for the final part.

---

### STEP 4 - Profiles, Known Crashes and Launching the game

#### 4.1 BFCO Gamepad Controls Fix, and Profile selection

Finally, everything should be in place.

If you plan to use one of the BFCO profiles, due to a clash between RaceMenu, Steam Input and Bethesda "helping", you will need to add `steamdeck=0` to the launch options in Steam:

<img src="https://github.com/Omni-guides/Tuxborn/blob/main/images/Tuxborn_SteamDeck0.png" width="600">

You should also temporarily map the 'R' key so that you can initiate the Character Naming pop-up during character creation. You could for example map it to one of the back buttons. This is only needed for Character Creation. You can thank Todd for this requirement.

With that done (or not if you are playing a non-BFCO profile), Start Tuxborn from Steam, and ModOrganizer2 should open.

Select your desired profile in the top-left of MO2 - as a reminder there are 6 profiles in total, with 4 of them being targeted at the Steam Deck. They are:

<img src="https://github.com/Omni-guides/Tuxborn/blob/main/images/Tuxborn_SelectProfile.png" width="600">

**Tuxborn – Deck:** This profile aims for a locked 40FPS experience on the Steam Deck.  
**Tuxborn - Deck CS:** This profile aims for a locked 30FPS experience on the Steam Deck, but with the additional visual benefits of the Community Shaders mod and profile.  
**Tuxborn – Desktop:** This profile is for slightly more powerful PCs, has an expanded Community Shaders suite and higher INI settings. Performance of this profile will depend on your system specs.  

**Tuxborn – Deck BFCO:** This profile aims for a locked 40FPS experience on the Steam Deck, and includes the BFCO Combat Animation Framework.  
**Tuxborn - Deck CS BFCO:** This profile aims for a locked 30FPS experience on the Steam Deck, but with the additional visual benefits of the Community Shaders mod and profile, and includes the BFCO Combat Animation Framework.  
**Tuxborn – Desktop BFCO:** This profile is for slightly more powerful PCs, has a full Community Shaders suite, higher INI settings, and includes the BFCO Combat Animation Framework. Performance of this profile will depend on your system specs.  

Once you have made your choice, select it in the Profiles drop down.

#### 4.2 Launching the game

Regardless of which profile you want to use you should now, finally, be ready to click play. Unfortunately, there are a couple of 'initial launch' issues that you will need to go through, but once these are out the way, they should never re-appear.

First point to note is the 'Unlock' button that will appear shortly after you click Play. Never, ever (ever) click the Unlock button.

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/TuxbornFull/UnlockButton" width="600">

⚠️ ❗ UNDER NO CIRCUMSTANCES PRESS THE “UNLOCK” BUTTON WHEN YOU HAVE LOADED SOMETHING THROUGH MOD-ORGANIZER.
YOU WILL BREAK MANY MANY THINGS. DO NOT PRESS THE BUTTON! ⚠️ ❗

Second thing to note, is the time it takes to boot the game. It takes a long, long (long) time to boot the game on Steam Deck. This has only been made worse with some recent changes to SteamOS. It can literally take 10+ minutes for the game to fully launch on Steam Deck (See [Additional Notes](https://github.com/Omni-guides/Tuxborn/blob/main/TuxbornSteamDeckFullInstall.md#additionals-notes) for some examples of timings). Rest assured we are looking into any possible way we can reduce this because it's a massive pain in the... As soon as we have anything that will help reduce this loading time, we will implement it. Running Tuxborn from SDCard will only make this initial load time worse, but it _will get there_, and regardless of internal storage or SD Card, once it's loaded, it will be fine.

Thirdly, there are a series of crashes the first few times you launch the game. This is something to do with running Tuxborn via Proton. Again, we are actively looking into anything we can do to reduce or remove the couple of crashes the first few times you launch Tuxborn.

The very first launch will likely crash fairly early, during the shader compilation. The second launch will take care of the initial Shader Cache building, and will again **take a very long time**. This should be a one-off though, so just let it complete. It will likely crash again at the end of that process.

Finally, though, things will start to smooth out. However, while the game is loading, the main menu background may be incredibly weird colours, e.g:

<img src="https://github.com/Omni-guides/Wabbajack-Modlist-Linux/blob/main/images/TuxbornFull/MainMenuCorruptColours.png" width="600">

This is caused by a different shader building process, and it will sort itself out when the game fully launches, and hopefully will stop happening after the first few launches.

Finally (finally), Tuxborn should now boot to the main menu options, no more crashes, no more nonsense. Once you reach this stage where things are settled, exit the game and switch back to Game Mode on the deck, and get playing!

### Additionals Notes

#### Install times with various storage combinations
I did some testing on my LCD Steam Deck to see how long a full Tuxborn install took to complete. This **doesn't** include the time to download all mods, because that is entirely dependant on your internet speed.

Tuxborn Wabbajack Deck Install times:

```
Internal Storage Install Diretory AND Downloads Directory: 4 Hours 6 Minutes
Internal Storage Install Directory and SDCard Downloads Directory: 2 Hours 26 Minutes
Internal Storage Downloads Directory and SDCard Install Directory: 8 Hours 10 Minutes
SDCard Install Directory and Downloads Directory: 10 Hours 31 minutes
```

As you can see, it can take a long time to complete the install using the Deck hardware alone, with the fastest options being having the Install Directory on Internal Storage, and Downloads on SDCard, or both Install Directory and Downloads Directory being on the Internal Storage.

#### Tuxborn Launch times with different Profiles

As mentioned in the main body of this guide, it can take a long time for Tuxborn to fully load on the Steam Deck hardware. To give you an idea of differences between the profiles and storage, I ran some tests:

```
Tuxborn Deck boot NVMe: 9m32s
Tuxborn Deck CS boot NVMe: 10m54s

TuxBFCO Deck boot NVMe: 9m45s
TuxBFCO Deck CS boot NVMe: 10m58s
```

It would be interesting to see if anyone has vastly different timings from the above.


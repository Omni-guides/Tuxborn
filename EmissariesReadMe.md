![Hello](https://github.com/Omni-guides/Tuxborn/blob/main/images/Emissaries%20of%20Tux.png)

# About

Emissaries of Tux is a performance friendly Wabbajack list for the english Steam version of Enderal SE, aiming to give the world of Vyn a more unique feel over Skyrim, targeting at minimum the hardware of the Steamdeck. A lot of work, including custom patches, have been placed to overhaul some of the skyrim looking elements. Together with mods adding extra content to the world like the Kata series of mods and Forgotten Dungeons series. While remaining friendly to the first time player in the world of Vyn. With a total install size of 55gb and a download of 41gb.

For those unfamiliar with Enderal, it’s a total overhaul for Skyrim made by the German game studio SureAI. There are 4 games in the setting of Vyn, but you don’t need to play the previous 3 to get into Enderal. Depending on who you ask, it might even be better to jump in blind. Not only have the world and story be reworked but also the gameplay. The Enderal world is de-leveled and you will need to buy skill books to level up your skills. Healing in combat comes with some minor drawbacks, similar to the rad system of Fallout, but there are also many powerful items to find around the world. While you sometimes will have to come back to stuff later with a more powerful character, there is always a way to overcome what you encounter.

If you wish to chat about Emissaries of Tux, join the [Aetherius Modding Discord](https://discord.gg/xRrHRsb5e9), grab the Tuxborn role from Channels & Roles and look for us in the #txbn-general or #txbn-support if you need help with something (do use the Enderal tag to help us with what list you are running). Or if you just want to chat about Wabbajack Modlists on Steam Deck/Linux in general, then drop by the #unofficial-linux-help channel of the [Official Wabbajack Discord](https://discord.gg/wabbajack).

For Wabbajack instuctions you can look here https://github.com/Omni-guides/Tuxborn/blob/main/README.md#wabbajack 

### <ins>Performance</ins>

As noted above, Emissaries of Tux is designed for the performance profile of the Steam Deck, but that doesn’t mean it’s limited to that platform! It’s also a great, content-full, lightweight (in terms of performance) list for less powerful systems. That is why there are multiple profiles, but you can run the same save across all of them. 

**Emissaries of Tux -  Deck:** This profile aims for a locked 40FPS experience on the Steam Deck. Comes with part of the CS set-up.

**Emissaries of Tux - CS:** Same as Deck, but with all the CS addons that are released at this point in time. This profile is for more powerful PCs.

**Emissaries of Tux - CS lite:** A profile in between Deck and CS.

**Emissaries of Tuxborn – ENB:** Replaces CS with Ambrosia ENB, where this one or CS will run better will be system dependent. 

Please Note: Due to the need for shader cache building on the Steam Deck, there may be a noticeable stutter in the first 1-2 hours while the cache builds. It should be good after that.

### <ins>Deck/Linux</ins>

TBA - Is being worked on but Omni has a lot of plates spinning at the moment. If you are a bit more experienced with Linux gaming you can set up the list now using these instructions: https://github.com/Omni-guides/Wabbajack-Modlist-Linux/wiki/General-Linux-Guide-(Anvil), with the these launch options https://github.com/Omni-guides/Wabbajack-Modlist-Linux/wiki/FNVTemp#step-5---set-the-required-launch-options-in-steam - replace 22380 with 976620.

### <ins>Optional Mods</ins>

**Custom Presets Go in Here:** An empty folder to put any custom racemenu presets in (.jslot file format).

**SSE FPS Stabilizer:** A SKSE plugin that dynamically changes settings based on a performance target, can be disabled if you run into weird performance issues.

**Bigger HUD:** Makes the HUD bigger in scale for small screens.

**Frame Generation - ENB Frame Generation:** A in engine frame gen option, don’t use it together with any other sources like lossless scaling or AFMF.

**Masculine Animations for Female PCs/Feminine Animations for Male PCs:** changes some animations for the Player Character.

**Story Mode - not safesave:** Makes the game easier for those that want it, as Enderal is more challenging then default Skyrim. This will only work properly on a new save, make sure you enable the esp - it's to keep it at the bottom of the loadorder.

### <ins>Framegen and Upscalling with CS</ins>

To toggle these on  you need to use the CS menu in game by hitting END key, see here how to do that with controller/handhelds: https://github.com/Omni-guides/Tuxborn/wiki/Community-Shaders-on-handheld-devices. On the left you will see a list of options, you want upscalling under the header display. Where you see TAA is where you can toggle upscalling between FSR and DLSS, lower down on the page you have options for framegen.

**When to use upscalling:**
Upscalling renders the game at a lower resolution and then uses ai to make it look higher res. You should use this if you aren't getting a stable 30fps (if you are running consistently below that switch to another profile) or you want to conserve some power when you are running on a handheld/laptop. 

**When to use framegen:**
Framegen uses ai to add fake frames to make the game feel more smooth, at the cost of higher input latency. You should only use this when you are already running between 40-50fps. It should roughly double your fps, when you use this on a screen that runs lower than 120fps you also need to toggle the force framegen option. 

You can use CS upscalling and framegen together, but you should expect to see some artifacting. DON’T use them together with external sources, like lossless scaling. 

### <ins>Downloads that some times fail</ins>

If wabbajack fails to grab these files use the links below and place the files in your seleceted download folder

Mod.Organizer-2.5.2.7z - https://github.com/ModOrganizer2/modorganizer/releases/download/v2.5.2/Mod.Organizer-2.5.2.7z

Synthesis.zip - https://github.com/Mutagen-Modding/Synthesis/releases/download/0.34.0/Synthesis.zip

EnderalSEEdit - https://www.nexusmods.com/enderalspecialedition/mods/78?tab=files&file_id=2793

### <ins>Beginner Tips for Enderal</ins>

After meeting Jespar, go check out the camp/region you just came from and after that go directly to Riverville. Swimming in the river is the safest way.

Riverville will be your homebase during the first act and don’t forget to make use of the many merchants there, especially buying skill books is important.

During the early game it can be helpful to make potions to get some extra experience and money, even if you don’t invest in the skill.

Food is your friend and will give you long lasting healing, be sure to collect all the meat and salt you can find. These can then be turned into meals at a cooking station, you can find one in the Riverville Inn.

Focus on 3-4 main skills and 1-2 crafting skills when making your character

Enderal has its own [Wiki](https://en.wiki.sureai.net/Enderal) if you feel stuck or want to check something

### <ins>Keybind Changes/Gamepad buttons</ins>

Heromenu is an important part of Enderal and is where you can see your skills among other stats, normally you can use it by pressing H. But in Emissaries it has been moved to the tween menu, in the same place as you find the level menu in normal Skyrim. You can map the shortcut for it in same place as other Skyrim controlles.

### <ins>Known issues to be aware of:</ins>
The Darkwoods area can be really heavy on the Steam Deck and the roof of the castle in particular, so you might want to turn on Frame Generation when in there. Toggling the Frame Generation is a 100% safe save.

The racemenu camera can be a bit claustrophobic, you can tweak the camera in one of the other racemenu tabs.

Sometimes you still get the heromenu tutorial at higher levels, you can turn this off in the Enderal mcm.

Chests lack opening animations that is because Medieval Chests doesn't have them at this point in time.

Controlers sometimes don't seem to work with Eot on windows, hit the XBOX/GUIDE or similar button ones when in game and that will fix it. 

### <ins>Installing your own mods</ins>

Your are free to install you own mods into Emissaries of Tux, but this voids your offical support. If you do still want/need help look for the modlist-modifications channel in the discord. It's highly recommended that you look at these guides before you make any changes [Lively's modding wiki](https://github.com/LivelyDismay/Learn-To-Mod/wiki) and [Althro's resources](https://github.com/The-Animonculory/Modding-Resources)

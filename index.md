## RB3Enhanced

RB3Enhanced (Rock Band 3 Enhanced) is a Rock Band 3 Dashlaunch plugin for RGH Xbox 360 consoles that aims to provide extra features and patch the game to facilitate easier file modifications.

This plugin is **not** intended to faciliate piracy, nor does it make _any_ attempt at facilitating it. It's simply a collection of features and patches intended to enhance the RB3 experience. Please support Harmonix and buy your DLC legally! The majority of it is still for sale on the Xbox Live Marketplace.

### Requirements

RB3Enhanced requires the following:
* An RGH/JTAG Xbox 360 running Dashlaunch - it is totally untested on a devkit and very likely won't work on one
* Rock Band 3 NTSC manually patched to Title Update 5 using Xextool - see Installation Tutorial for more info on this

### Features
* Song blacklist removal, allowing Hier Kommt Alex and Rock N' Roll Star to be playable once more
* Removal of ARK checksums, allowing modification of all game files
* Using an arbitrary game_origin no longer breaks the VENUE track in songs, allowing for new game_origins to be used in songs.dta
* Forces the game to load patch_xbox.hdr and patch_xbox.ark from Rock Band 3's main /gen/ directory instead of looking for it in the TU5 STFS package
* CON check removal, allowing custom songs in the CON format to work in TU5
* Song speed selector ala Clone Hero [(preview)](https://www.youtube.com/watch?v=BuXSdth-_Vo)
* Play 5-lane keys on guitar controllers without needing to have the goal unlocked
* Change the scroll speed of all instrument tracks to anything you prefer
* Force your virtual band to always play on a specific in-game venue, or load a simple black background instead of any venue which cuts loading times significantly

Plus more features I have probably forgotten to list here. Take a look through the rb3.ini file to see all the configurable settings.

### Planned Features
* "Corona fix" to stop the game from having issues on Corona motherboards
* File loader to load files from the HDD instead of from the ARK file
* Wacky "why not" features like playing drums charts on guitar and vice versa, or two bassists/guitarists at once
* Overlapping sustains and open strum notes ala Guitar Hero
* Per-song loading of custom sound banks, allowing things like custom drum/percussion SFX

## Download
RB3Enhanced can be downloaded via [this Mediafire link](https://www.mediafire.com/file/ky65kqu9c5o88tt/RB3Enhanced_0.3.0.1.zip/file). Alternatively, you can find the latest version in the #rbhax channel in the [MiloHax discord server](https://discord.gg/QKe7vRnJG3).

### Changelog
The latest version of RB3Enhanced is version 0.2. See the changelog [here](https://ihatecompvir.github.io/RB3Enhanced/changelog).

## Installation Tutorial
Installing RB3Enhanced is as simple as installing any other Dashlaunch plugin.
- Copy RB3Enhanced.xex to somewhere on your hard disk or USB flash drive and modify launch.ini to add it as a plugin in Dashlaunch, similar to installing XBDM.xex or another commonly used Dashlaunch plugin. The order in which you add the plugin does not seem to matter
- Manually patch RB3 to TU5 using Xextool. Get your RB3 default.xex and the default.xexp for TU5, and run the Xextool command "xextool -p default.xexp default.xex" to patch RB3 to TU5. Then just copy the patch_xbox.hdr and patch_xbox.ark files into RB3's main /gen/ folder.

### Common Questions
* **Q: Does this work on XBL?**
* A: Possibly, but please don't get on XBL on a modded console.

* **Q: Does this work on Xenia?**
* A: RB3Enhanced has been tested on Xenia and it does not work. Without getting too technical, RB3Enhanced makes patches to code in real-time, something that does not seem to be supported on Xenia. It may be supported one day as Xenia becomes more accurate, but this is probably a long ways away, if ever.

* **Q: Can you add support for X Rock Band game?**
* A: While this is intended to support Rock Band 3, I have been considering adding at least a basic featureset for other titles, specifically the removal of ARK checksums. Keep your eyes peeled for future updates.

* **Q: Can you make this for PS3?**
* A: I have no experience with PS3 development, so I cannot. That being said, once the source code is released, anyone is free to port it to PS3 and if a PR is submitted, I would gladly merge it. There is no technical reason why RB3Enhanced couldn't be ported to PS3 as an SPRX plugin or similar for jailbroken consoles.

* **Q: Can you make this for Wii?**
* A: Some preliminary work has been done for porting certain features to Wii, so a Wii port is still being looked into. Stay tuned.

* **Q: Can you add X feature?/I found a bug, where do I report it?**
* A: I am definitely interested in hearing about new features that would be useful. Please reach out to me on Twitter @ihatecompvir or Discord @ihatecompvir#1863 for any feature suggestions or bug reports.

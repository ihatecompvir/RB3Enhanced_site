## RB3Enhanced

RB3Enhanced (Rock Band 3 Enhanced) is a Rock Band 3 Dashlaunch plugin for RGH Xbox 360 consoles that aims to provide extra features and patch the game to facilitate easier file modifications.

This plugin is **not** intended to faciliate piracy, nor does it make any attempt at facilitating it. It's simply a collection of features and patches intended to enhance the RB3 experience. Please support Harmonix and buy your DLC legally! The majority of it is still for sale on the Xbox Live Marketplace.

### Requirements

RB3Enhanced requires the following:
* An RGH/JTAG Xbox 360 running Dashlaunch - it is totally untested on a devkit and very likely won't work on one
* Rock Band 3 NTSC manually patched to Title Update 5 using Xextool - see Installation Tutorial for more info on this

### Features
* Song blacklist removal, allowing Hier Kommt Alex and Rock N' Roll Star to be playable once more
* Removal of ARK checksums, allowing modification of all game files
* Using an arbitrary game_origin no longer breaks the VENUE track in songs, allowing for new game_origins to be used in songs.dta
* Forces the game to load patch_xbox.hdr and patch_xbox.ark from Rock Band 3's main /gen/ directory instead of looking for it in the TU5 STFS package

### Planned Features
* "Corona fix" to stop the game from having issues on Corona motherboards
* Song speed selector ala Clone Hero [(preview)](https://www.youtube.com/watch?v=BuXSdth-_Vo)
* CON check removal, allowing custom songs in the CON format to work in TU5
* File loader to load files from the HDD instead of from the ARK file
* Song limit removal patch done in real-time without having to modify DTAs

## Download
RB3Enhanced can be downloaded via [this Mediafire link](https://www.mediafire.com/file/juapb1b8ez9ipx9/RB3Enhanced_0.2.zip/file). Alternatively, you can find the latest version via the Pinned message on the #rbhax channel in the [MiloHax discord server](https://discord.gg/QKe7vRnJG3).

## Installation Tutorial
Installing RB3Enhanced is as simple as installing any other Dashlaunch plugin.
- Copy RB3Enhanced.xex to somewhere on your hard disk or USB flash drive and modify launch.ini to add it as a plugin in Dashlaunch, similar to installing XBDM.xex or another commonly used Dashlaunch plugin. The order in which you add the plugin does not seem to matter
- Manually patch RB3 to TU5 using Xextool. Get your RB3 default.xex and the default.xexp for TU5, and run the Xextool command "xextool -p default.xexp default.xex" to patch RB3 to TU5. Then just copy the patch_xbox.hdr and patch_xbox.ark files into RB3's main /gen/ folder.

### Common Questions
* **Q: Does this work on XBL?**
* A: Possibly, but please don't get on XBL on a modded console.

* **Q: Does this work on Xenia?**
* A: As Xenia doesn't even run RB3 properly yet, the answer is no. In theory, though, it may one day be compatible once RB3 is supported and if Xenia decides to add support for loading Sysdlls.

* **Q: Can you add support for X Rock Band game?**
* A: While this is intended to support Rock Band 3, I have been considering adding at least a basic featureset for other titles, specifically the removal of ARK checksums. Keep your eyes peeled for future updates.

* **Q: Can you make this for PS3?**
* A: I have no experience with PS3 development, so I cannot. That being said, once the source code is released, anyone is free to port it to PS3 and if a PR is submitted, I would gladly merge it.

* **Q: Can you make this for Wii?**
* A: I don't think it is even possible to load an extra process into memory on Wii in the way that it is possible on PS3 or 360, so no. I might be wrong here, but it seems it would be very challenging to port this to Wii.

* **Q: Can you add X feature?/I found a bug, where do I report it?**
* A: I am definitely interested in hearing about new features that would be useful. Please reach out to me on Twitter @ihatecompvir or Discord @ihatecompvir#1863 for any feature suggestions or bug reports.

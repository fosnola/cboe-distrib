I compiled this version with XCode version 13.2.1, so I guess it can only work on OsX 10.9 and above (I currently use macOS Big Sur). 

====================== IMPORTANT ================================
These executables are not signed, so you will have to force GateKeeper to run them. 
On OSX High Sierra/../Big Sur, the only solution I found is to run these commands in the terminal:

cd ~/Downloads/BoE-experimental-MacIntel64-unstable
xattr -d com.apple.quarantine BoE\ Character\ Editor.app/
xattr -d com.apple.quarantine BoE\ Scenario\ Editor.app/
xattr -d com.apple.quarantine Blades\ of\ Exile.app/

If you do not run these commands, the applications will probably CRASH with the following exception:
ticpp::Exception: Couldn't load /private/var/folders/XXX/YYYY/T/AppTranslocation/ZZZZ/d/data/dialogs/1str-title.xml

===================== Notes =====================================
- this version corresponds to an unstable version https://github.com/fosnola/cboe ( branch monsterCode )
  commit 81e8d3ece7a3f03346374b264e1907d18cd4c9da
- concerning the graphics, I put in data/graphics the original graphics,
  and in data/graphics2 the graph I used to test cboe. If you want to test them, 
  you can rename data/graphics to data/graphics_original and data/graphics2 to data/graphics


===================== THIS VERSION IS EXPERIMENTAL ===============
============= MUST NOT BE USED TO CREATE A NEW SCENARIO ==========

- the version is experimental and unstable, it differs from the "classical" cboe sources by :
  + a junk bag can be enabled in the preferences,
  + I totally changed the method to store special nodes; this new method seems interesting: it is more powerful and we can add new functions more easily. However, it changes the file format of the .boes files and some standardization work clearly needs to be done. So you should not use this experimental version if you want to create a new scenario.
  + I just add the possibility to add code using templates for scenario/town/outdoor specials ( but the code is not really tested )
  + I change the sources to display utf8 characters, this can allow to translate some scenarios.
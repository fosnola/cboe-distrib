I compiled this version with XCode version 13.2.1, so I guess it can only work on OsX 10.9 and above (I currently use macOS Big Sur). 

====================== IMPORTANT ================================
These executables are not signed, so you will have to force GateKeeper to run them. 
On OSX High Sierra/../Big Sur, the only solution I found is to run these commands in the terminal:

cd ~/Downloads/BoE-MacIntel64-Jan2022
xattr -d com.apple.quarantine BoE\ Character\ Editor.app/
xattr -d com.apple.quarantine BoE\ Scenario\ Editor.app/
xattr -d com.apple.quarantine Blades\ of\ Exile.app/

If you do not run these commands, the applications will probably CRASH with the following exception:
ticpp::Exception: Couldn't load /private/var/folders/XXX/YYYY/T/AppTranslocation/ZZZZ/d/data/dialogs/1str-title.xml

===================== Notes =====================================
- this version corresponds to https://github.com/fosnola/cboe
  commit 4f4770f3786a54720a5cc9fbd55a159ae2e741a2
  (+ a "merge" still not committed of the second part of 97f0723a4c69580457a4e1ba4b0ff60ecd4e2621 https://github.com/Terane346/cboe)
- concerning the graphics, I put in data/graphics the original graphics,
  and in data/graphics2 the graph I used to test cboe. If you want to test them, 
  you can rename data/graphics to data/graphics_original and data/graphics2 to data/graphics

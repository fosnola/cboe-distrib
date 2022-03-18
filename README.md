# cboe-distrib
Repository to store the latest distributions of Classic Blades of Exile see https://github.com/calref/cboe


This project hosts some executables of the classic RPG creator Blades of Exile after it was released by Spiderweb Software under GPLv2. The source code can be found either at https://github.com/calref/cboe or at https://github.com/fosnola/cboe.

Currently, it contains:
- MacOsX/OsX11-MacIntel64.zip: Intel 64 OsX executables compiled from https://github.com/fosnola/cboe in Big Sur for MacOsX 10.9 - 10.11, as these executables are unsigned, you must first read the **ToReadBeforeLaunching.txt** which explains how to bypass GateKeeper.
- MacOsXExperimental/OsX11-MacIntel64.zip: Intel 64 OsX executables compiled from the branch *special_code* of https://github.com/fosnola/cboe in Big Sur for MacOsX 10.9 - 10.11, as these executables are unsigned, you must first read the **ToReadBeforeLaunching.txt** which explains how to bypass GateKeeper. This version differs from "classical" cboe sources by:
  + a **junk bag** can be enabled in the preferences,
  + I totally changed the method to store special nodes; this new method seems interesting: it is more powerful and we can add new functions more easily. However, it changes the file format of the .boes files and some standardization work clearly needs to be done. So you should not use this experimental version if you want to create a new scenario.
  + I change the sources to display correctly utf8 characters which can allow to translate some scenarios. To test it, I translated quickly valleydy.boes in french, my poor translation appears in Blades\ of\ Exile\ Scenarios/ValléeMourante.boes. You have to copy it in the Scenarios repository : ~/Library/Application\ Support/Blades\ of\ Exile/Scénarios/ if you want to launch it. 


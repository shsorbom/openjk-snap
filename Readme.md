# Snap Package for the OpenJK Project
The OpenJK project maintains the engine of the "Jedi Academy" and "Jedi Outcast" games, originally made by Lucas Arts

This repository packages their work for the Ubuntu Snap pachage format

## What you will need to use this project
* Any major Linux Distribution, Circa 2016 or newer
* Snapcraft -- Ships with all major Linux Distributions
* Original copy of the game data for "Jedi Academy" and "Jedi Outcast"
* Modern-ish intel GPU (tested on Haswell)
* Basic Linux command line skills

## Building and Running this Project
* Install the snapcraft program (Methods vary here, consult distro documentation)
* Open a terminal
* Type "snapcraft"
* Run "snap install --dangerous --devmode ./openjk_0.1_amd64.snap" in the directory of the .snap file
* Put game data in ~/snap/openjk/.local/share/JediAcademy/base
* Run "openjk.openjk-sp" at terminal (for single player)

## Notes
* Has not been tested on NVidia or AMD GPUs
* There are no desktop shortcuts right now
* Jedi Outcast is not buit by default yet, future commits will enable it (I will also accept pull requests :) )

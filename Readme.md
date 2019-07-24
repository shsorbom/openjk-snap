<h1 align="center">
  <img src="snap/gui/OpenJK_Icon_256.png" alt="OpenJK">
  <br />
  OpenJK
</h1>

# Snap Package for the OpenJK Project
The OpenJK project maintains the engine of the "Jedi Academy" and "Jedi Outcast" games, originally made by Lucas Arts

This repository packages their work for the Ubuntu Snap pachage format

[![Open Jedi Knight](https://snapcraft.io/openjk/badge.svg)](https://snapcraft.io/openjk)

## What you will need to use this project
* Any major Linux Distribution, Circa 2016 or newer
* Snapcraft -- Ships with all major Linux Distributions (only for building)
* Original copy of the game data for "Jedi Academy" and "Jedi Outcast"
* Modern-ish intel GPU (tested on Haswell)
* Basic Linux command line skills

## Installing
On 64-bit Architecture:

    sudo snap install openjk
On all other Architectures:

    sudo snap install --edge openjk

## The Game Assets
Openjk is built on the quake III Engine, and as such all of the game assets are packaged in PK3 (.pk3) format.
These files do not come with the openjk project and must be obtained from original game copies
The original game can be purchased from Gog.com or from the Steam store

Once you have them, the PK3 files need to be placed in:
    ~/snap/openjk/<revision>/.local/openjk/base
for Jedi Academy, or
    ~/snap/openjk/<revision>/.local/openjo/base
for Jedi Outcast.

## The Binaries
This package contains four binaries:
**openjk** -- The binary for Jedi Academy Multiplayer games
**openjk-sp** -- The binary to play the Jedi Academy single player campaign
**openjo-sp** -- The binary to play the Jedi Outcast single player campaign
**openjkded** -- The binary to run a dedicated, headless Jedi Academy Multiplayer Server
Commannnnd line options for the Server are specified using the "+" delimeter

## Building and Running this Project Yourself (No longer required)
* Install the snapcraft program (Methods vary here, consult distro documentation)
* Open a terminal
* Type "snapcraft"
* Run 

    snap install --dangerous ./openjk_1.0.1.1_amd64.snap 


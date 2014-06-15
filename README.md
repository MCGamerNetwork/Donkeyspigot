Donkeyspigot [![Build Status](https://travis-ci.org/SpigotMC/Spigot.png)](https://travis-ci.org/SpigotMC/Spigot)
===========

Fork of Spigot, the high performance Minecraft server implementation, with support for Donkeychunk, the highly space efficient level storage format.

How To
-----------

Init a Craftbukkit and Bukkit module : `git submodule update --init`

Apply Patches : `./applyPatches.sh`

[Download the Donkeychunk library by clicking here.](https://github.com/MCGamerNetwork/Donkeychunk) You'll need it to compile Donkeyspigot.

### Create patch for server ###

`cd Spigot-Server`

Add your file for commit : `git add <file>`

Commit : `git commit -m <msg>`

`cd ..`

Create Patch `./rebuildPatches.sh`

### Create patch for API ###

`cd Spigot-API`

Add your file for commit : `git add <file>`

Commit : `git commit -m <msg>`

`cd ..`

Create Patch `./rebuildPatches.sh`




Compilation
-----------

We use maven to handle our dependencies.

* Install [Maven 3](http://maven.apache.org/download.html)
* Clone this repo and: `mvn clean install`

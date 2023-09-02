# OpenSC2K
OpenSC2K - An Open Source remake of SimCity 2000 written in JavaScript, using WebGL Canvas and [Phaser 3](https://github.com/photonstorm/phaser/).

## Overview
Currently a lot remains to be implemented but the basic framework is there for importing and viewing cities. Lots of stuff remains completely unimplemented such as the actual simulation, rendering of many special case tiles and buildings and anything else that exists outside of importing and viewing.

Along with implementing the original functionality and features, I plan to add additional capabilities beyond the original such as larger city/map sizes, additional network types, adding buildings beyond the initial tileset limitations, action/history tracking along with replays and more.

I've only tested using Chrome / Firefox on macOS, but it should run fairly well on any modern browser/platform that supports WebGL. Performance should be acceptable but there is still a LOT of room for optimizations and improvements.

Due to copyrights, the original graphics and assets from SimCity 2000 cannot be provided here. I've developed and tested using the assets from SimCity 2000 Special Edition for Windows 95. Once I've got the basic engine stabilized I plan to add support for multiple versions of SimCity 2000 in the future.

**Update:** I've been working on refactoring considerable portions of the code for clarity and performance. Due to the changes a lot of existing functionality is now completely broken and will be fixed in upcoming commits.

![Screenshot](/screenshots/1.png)

## Installation
You can use yarn (recommended) or npm to install and run. Once installed and started, open a browser to http://localhost:3000 to start the game.

### OS X / Linux
1. `git clone ` or download this repository
1. `cd OpenSC2K`
1. `yarn install` downloads and installs the dependancies
1. `yarn dev` to run

## Usage
By default, a test city included in the /assets/cities/ folder will load. Currently you must modify the `/src/city/load.js` file to load different cities.

Requires two files from the Windows 95 Special Edition version of SimCity 2000: `LARGE.DAT` and `PAL_MSTR.BMP`. These must be placed in the `/assets/import/` directory prior to starting the game. The files will be automatically parsed and used for all in game graphics.

### Controls
 - `WASD` to move the camera viewport
 - `Q` or `E` to adjust camera zoom

![Screenshot](/screenshots/2.png)
![Screenshot](/screenshots/3.png)
![Screenshot](/screenshots/4.png)


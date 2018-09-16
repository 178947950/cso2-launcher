# cso2-launcher
[![Build status](https://ci.appveyor.com/api/projects/status/ajl6d1ir9s3l4lyu/branch/master?svg=true)](https://ci.appveyor.com/project/Ochii/cso2-launcher/branch/master)

A modified client for Nexon's (South Korea) Counter-Strike: Online 2.

## How to use
**This tool requires a copy of Nexon's Counter-Strike: Online 2.**
**It also needs incomplete [emulated master server](https://github.com/Ochii/cso2-master-server/) running in order to work.**

You may get one [here (MEGA)](https://mega.nz/#!nhgnBJgD!iR57D5Mf3_1GCcAR36tqFQ7H7KN_F0e3XicD2JBoSN4) or [here (Google Drive)](https://drive.google.com/open?id=1y0diL2nTERlOaJZQTA3xPb8owx82GjtB) (SHA-256: 02F76DBDD083EF78ECC92EB963C7C7A7576FF2E2C695671A4F358C2580584965).

Then, download a copy of the project [here](https://github.com/Ochii/cso2-launcher/releases) (it will connect to ```127.0.0.1```, or your local machine, if you prefer) and copy the contents of the compressed file to ```[your CSO2 game path]/Bin```.

To start, run ```launcher_main.exe```. Once the game loads enter some login information - only your username will be taken into account.

When you're done logging in, you can host a room. Choose the second option in the menu that reads *공식전* (has something to do with game seasons?), then pick any option.

At this point you may get more players in by repeating these steps, or start the match by pressing *게임 시작* (means roughly *game start*?). 

The match options are unchangeable, and you can't do almost anything else since the master server is incomplete.

There will be a console window where you can input commands just like a regular Source Engine console (you can enable ```cl_showfps```, for example).

## Bug reporting and improvements
Have a look at the [issues](https://github.com/Ochii/cso2-launcher/issues) for a list of bugs found or to report them yourself.

If you have any improvements that you would like to share or comment about, have a look at the [pull requests](https://github.com/Ochii/cso2-launcher/pulls).

## How to build

### Requirements
- [CMake](https://cmake.org/download/)
- [Visual Studio 2017](https://www.visualstudio.com/downloads/)
- [Windows PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-windows-powershell)

Only **Windows** is supported.

### Downloading the source code
Clone the project with ```git clone --recursive https://github.com/Ochii/cso2-launcher.git```.

### Before building
Start a PowerShell instance and change directory to the project's directory, then, run ```./setuplibs.ps1```.

The script will setup PolyHook, its dependency Capstone and the Source SDK.

### Building
Open the solution ```CSO2Launcher.sln``` and build it in your preferred configuration.

If built successfully, you will find your binaries inside ```out/bin/Win32/[your configuration]```.

## Libraries used
- **[PolyHook v2.0](https://github.com/stevemk14ebr/PolyHook_2_0/)** by [stevemk14ebr](https://github.com/stevemk14ebr)

## Credits
- [Valve Software](https://github.com/ValveSoftware/source-sdk-2013) for their SDK

## Thank you's (by no particular order)
- To **[UserU](https://www.youtube.com/user/GoodbyeSpy)**
- To **[SHI_KU](https://www.youtube.com/channel/UC2HZo-HFOuxmS6zWYPMD0hQ)**
- To **ReddUT** from [Counter-Strike Online Wikia](https://cso.wikia.com/)'s Discord
- To **Frostie** from [Counter-Strike Online Wikia](https://cso.wikia.com/)'s Discord 

## License
Read ```LICENSE``` for license information.

I'm not affiliated with either Valve and/or Nexon, neither I own Counter-Strike Online 2.

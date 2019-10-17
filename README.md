# XreaL
![XreaL](https://github.com/RobertBeckebans/RBQUAKE-3/raw/master/docs/xreal_scrnshot.jpg)

**The project is hosted at:** https://github.com/RobertBeckebans

**Report bugs here:** https://github.com/RobertBeckebans/RBQUAKE-3/issues

Uses code from the ioquake3 project ![ioq3](https://github.com/raynorpat/xreal/raw/master/docs/ioquake3_logo.png)


## GENERAL NOTES

A short summary of the file layout:

Directory                     | Description
:---------------------------- | :------------------------------------------------
RBQUAKE-3/base/                   | XreaL media directory ( models, textures, sounds, maps, etc. )
RBQUAKE-3/code/                   | RBQUAKE-3 source code ( renderer, game code for multiple games, OS layer, etc. )
RBQUAKE-3/code/tools/xmap         | map compiler ( .map -> .bsp ) (based on q3map)
RBQUAKE-3/code/tools/xmap2        | map compiler ( .map -> .bsp ) (based on q3map2)
RBQUAKE-3/code/tools/xmaster	  | master server
RBQUAKE-3/blender/          	  | Blender plugins for ase, md3, and md5 models


## LICENSE

See docs/COPYING.txt for all the legal stuff.


## GETTING THE SOURCE CODE AND MEDIA

This project's git repository can be cloned with the following instruction set: 

`
git clone https://github.com/RobertBeckebans/RBQUAKE-3.git
`


## COMPILING ON WINDOWS

NOTE: THIS IS REALLY OUTDATED......

1. Download and install the Visual Studio 2017 Community Edition.
2. Generate the VC2017 projects using Premake 5 by doubleclicking a matching configuration .bat file in the premake/ folder.
3. Use the VC13 solution to compile what you need: RBQUAKE-3/premake/RBQUAKE-3.sln

## MULTIUSER SUPPORT ON WINDOWS SYSTEMS

On Windows, all user specific files such as autogenerated configuration,
demos, videos, screenshots, and autodownloaded pk3s are now saved in a
directory specific to the user who is running XreaL.

On NT-based systems such as Windows XP, this is usually a directory named:
  "C:\Documents and Settings\%USERNAME%\Application Data\XreaL\"

On Windows Vista, this would be:
  "C:\Users\%USERNAME%\Application Data\XreaL\"

Windows 95, Windows 98, and Windows ME will use a directory like:
  "C:\Windows\Application Data\XreaL"
in single-user mode, or:
  "C:\Windows\Profiles\%USERNAME%\Application Data\XreaL"
if multiple logins have been enabled.

You can revert to the old single-user behaviour by setting the fs_homepath
cvar to the directory where XreaL is installed.  For example:
  xreal.exe +set fs_homepath "c:\xreal"
Note that this cvar MUST be set as a command line parameter.
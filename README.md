# Mod Loader

Mod Loader is a plugin for Grand Theft Auto III, Vice City and San Andreas that adds an easy and user-friendly way to install and uninstall modifications into the game, as if the game had official modding support. No changes are **ever** made to the original game files, everything is injected on the fly, at runtime!

The usage is as simple as inserting the mod files into the *modloader/* directory. Uninstalling is as easy as that too, delete the mod files and you are done. Hot swapping mods while the game is running? By using Mod Loader you can!

### Building and Installing

Requirements:

+ [Premake 5](http://industriousone.com/premake/download) *(pre-built executable available in this repository root)*
+ [Visual Studio](http://www.visualstudio.com/downloads) 2013 or greater.

Run the following command in the root of this directory to generate the project files:

    premake5 vs2013

You can install the generated binaries into your game directory by running:

    premake5 install "C:/Program Files (x86)/Rockstar Games/GTA San Andreas"

Or, you might want the files to be automatically installed everytime you build the solution:
 
    premake5 vs2013 "--idir=C:/Program Files (x86)/Rockstar Games/GTA San Andreas"


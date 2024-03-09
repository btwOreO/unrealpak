# UnrealPAK

UnrealPak.exe is an official tool created by Epic as part of Unreal Engine 4. This version of the tool is from 2016 but it still creates PAK files which are compatible with seemingly any UE4 game (of the ones I've tested, anyway). And unlike other PAK creation tools I've found, this one can create compressed PAK files, which results in much smaller filesizes and, according to official UE4 documentation, faster loading.

Usage:
- Create a folder with mod contents (folder should be the name of the mod, and inside that should be the base folder for the game).
- Drag'n'drop the folder onto one of the batch files to create a PAK file.

There's also a batch file for unpacking unencrypted PAK files, but note that UnrealPak.exe ignores the base path for a PAK file during extraction, so chances are high you won't get the full path this way. It's recommended you use another tool for PAK unpacking.

Note that the tool might create a bunch of ini files at "..\..\Engine" when you run the tool. The tool is hardcoded to make these (probably because it's supposed to be used inside a UE4 project), but you can safely delete the ini files if they're created.

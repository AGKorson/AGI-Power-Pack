# AGI-Power-Pack
The AGI Power Pack is an AGI logic script that takes advantage of a bug in AGI's set.string command that allows modification of the program's executable code (basically a buffer overflow hack). The Power Pack leverages this to inject new assembly routines that significantly extend the capabilities of AGI. Since all of the code necessary to do this is contained entirely within the Power Pack logic code, it requires no modification to the AGI program files.

Because the Power Pack modifies the interpreter's code, it will only work on an original PC system running MSDOS or on a fully compatible MSDOS emulator, such as DOSBox. It will not work with any modern interpreters such as NAGI or SCUMMVM.

The assembly code that the Power Pack inserts into the interpreter is version dependent; each AGI interpreter needs its own logic code to make the Power Pack work, and they are not interchangeable. Power Pack logic source code is provided for all known version 2 and version 3 AGI interpreters.

The resources provided in the Power Pack repository include:
 - Power Pack Logic Source Code: a separate logic for each AGI version is provided in the PowerPack2 and PowerPack3 directories. To run the power pack, all you need to do is run the correct Power Pack Logic as the first thing in an AGI game. 
 - powerpack.txt: an #include file that contains pre-defined function names and constants that improve the readability of source code that uses Power Pack functions
 - pp_snippets.txt: a list of snippets that are compatible with WinAGI that make it easy to add Power Pack functions to logic source code; copy and paste the snippet entries into the snippets file in your WinAGI program directory to use these
 - Power Pack Mods.xlsx: an Excel spreadsheet that was used to create the Power Pack functions; all of the assembly code was developed using this spreadsheet
 - Power Pack Demo Game: the Demo game is a small (~10 room) AGI game that demonstrates some of the things you can do with the Power Pack; it includes very detailed comments in the source files that explains how to use the Power Pack functions that you can use to help create your own Power Pack enabled AGI games
 - Power Pack Test Game: two test games, PP2TEST and PP3TEST are included in the PPTEST directory; these games are a simple one room template game that runs all the Power Pack features through a battery of tests to confirm they work properly; you can examine these to gain additional insight in to how to use the Power Pack features in an actual AGI game

If you have any questions or comments, you can contact me in the AGI forums at https://sciprogramming.com/community/index.php.
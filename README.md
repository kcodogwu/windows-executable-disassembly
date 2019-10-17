# Windows Executable Disassembly

In this class assignment, I reverse-engineered a given Windows PE executable. I produced a summary of my approach to reverse engineering the executable, the purpose, content, and structure of each variable defined in the program used to create the executable, algorithms of user-written (non-standard) functions within the program, and a detailed de-obfuscation algorithm and equivalent C programming code, explaining the data de-obfuscation function and the de-obfuscated data produced as output. The `disassembly-of-a-windows-executable.md` file contains this summary.

Code snippets from the disassembled Windows PE executable can be found in the files:
* reverse-engineering-data.md: Containing Relevant snippets from the data region
* reverse-engineering-main.md: Containing code of the `_main` function
* reverse-engineering-sub-401000.md: Containing code of the `sub_401000` function
* reverse-engineering-sub-401080.md: Containing code of the `sub_401080` function
* reverse-engineering-sub-401160.md: Containing code of the `sub_401160` function

IDA Pro and OllyDbg were used in carrying out this reverse engineering exercise.

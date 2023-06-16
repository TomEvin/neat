<p align="center"><img src="/readme_assets/neat_icon.png" width="128"/></p>

<p align="center"><b>The tool is under development, planned release is about the publish of Alan Wake II. (with or without AW2 support, we will see then.)</b><br/> The documentation will update during the development process!</p>

>**This is a hobby project, so shits can happen during the usage of this tool, but virus and malware free!**
**The below mentioned tools has nothing to do with *Remedy Games / Remedy Entertainment* (not provided any support or code), the codebase developed by me!**

To run n^e^at you will need installed [.NET Desktop Runtime 6](https://dotnet.microsoft.com/en-us/download/dotnet/6.0). n^e^at developed to run on **Windows 11**, but Windows10 22H2 will be probably supported!

##About n^e^at
The tool was created for [Northlight Engine](https://www.remedygames.com/northlight/) Archive files to extract / repack / create.
The **Northlight Engine Archive Tool** (neat) is the rewritten version of the original **Alan Wake Tool** and later the **Northlight Tool**. None of those name cover now the real purpose and function of the tool, that's why I moved those function to a new and renamed project.

The Alan Wake Tool was created originally for Alan Wake Xbox360/PC only, to unpack archives and replace files inside them, mainly the localisation file.
<img src="/readme_assets/AlanWakeTool.png"/>

When the non-Alan Wake game was released (Quantum Break), using the name Alan Wake Tool was pointless, also the developers changed the name of the game engine from (non official) **Alan Wake engine**, to **Northlight**.
<img src="/readme_assets/NorthlightTool.png"/>

Because Northlight Engine Tool codebase is from Alan Wake Tool with little change and updated GUI, all the lacky coding and poor archive handling and reading was still present in the tool.
The tool **n^e^at** was built up from scratch and unlike its predecessors, rewritten completely in Object-oriented programming (OOP) way. Or at least I tried to.
The tool can read and create Northlight archive file (bin/rmdp). The repacked files are still not equal with the original files, but 99% of the time the game engine able to use the new archive file!
<img src="/readme_assets/neat_main.png"/>

###Features
- [x] Unpack archive files (bin/rmdp)
- [x] Create new archive file (bin/rmdp)
- [x] Convert binary text file to txt and back
- [x] Convert textures with .tex extension to DDS (DirectDraw Surface) format and back
- [x] Light / Dark mode (or following system setting)
- [ ] Different backgound image for each game
- [ ] Plan - Generate .packmeta, .xml companion files
- [ ] Will not support 3D files, media files etc. For those please check other solution, like [OpenAWE](https://github.com/OpenAWE-Project/OpenAWE)

###Supported games
(for up-to-date list please always check the description inside the tool)
| Game | Tested Platform | Development (Read/Write/Test) |
| ----------- | ----------- | ----------- |
Alan Wake | Xbox360 / PC | done/done/NA
Alan Wake's American Nightmare | Xbox360 / PC | under progress
Quantum Break | PC | under progress
Control | PS4 / PC | under progress
Alan Wake Remastered | PS4 / PC / NSW?! | done/done/NA
CrossfireX / Crossfire HD | XboxOne / SeriesX | under progress
Alan Wake II | PC | currently just plan!

---
##About Northlight Engine
Northlight is a game engine, created and developed by Remedy Entertainment.
The engine introduced with Alan Wake game in 2010 on Xbox360. Back then the engine had no public name, so everyone called it Alan Wake Engine. This was not changed until Quantum Break, when the engine was named officially to Northlight. On the surface, on the archivum/container file level, not much changed. This is why my tools (AW Tool, Northlight Tool, n^e^at) were/are backward compatible since first Alan Wake. Of course in the background the engine evolved since the beginning huge, added more and more new features.

The Northlight Engine games:
- 2010 - Alan Wake (under Alan Wake engine)
- 2012 - Alan Wake's American Nightmare (under Alan Wake engine)
- 2016 - Quantum Break
- 2019 - Control 
- 2021 - Alan Wake Remastered
- 2022 - CrossfireX / Crossfire HD (single-player)
- 2023 - Alan Wake II
- ???? - Control 2

[Northlight Engine](https://www.remedygames.com/northlight/)
[Remedy Games](https://www.remedygames.com)

<img src="/readme_assets/remedy_logo.png" alt="Remedy Entertainment" width="64"/>

---
##How to modding (not final)
The base concept of modding is to do not change the original files, but adding new contents or replace existing files with new archive files contain the updated engine files. So in this case create new archive files with minimal size.

The tool can unpack the main archive files (always the biggest ones), but not able to create a new, working one. Because the tool is not handling something correctly or the game protecting the files, I do not know, but it is not matter in case of modding.

So unpack all the bin/rmdp archive files (make sure you have enough free space for this step) and find the files you want to change. Modify them (ie. redraw textures) and place the modified files into a new folder with the correct folder/subfolder structure.
If you modify an unpacked file like: ep100-000-generic\folder1\folder2\texture.tex
Follow the folder structure in the new folder also: myNewFolder\folder1\folder2\texture.tex

If you not use the correct folders/subfolder and filenames, the game won't use the modified files from the mod container!

For the new file the name is also very important. If you unpacked from (Control game) ep100-000-generic archive, you HAVE TO use this name, but increase the number of the filename, like ep100-00**1**-generic. If there is already a "001" then increase until the file is not exist.

Examples:
ep100-000-generic-en -> ep100-00**1**-generic-en
ep100-000-pc -> ep100-00**1**-pc
ep101-000-pc -> ep101-00**1**-pc

**More details later...**

---
##n^e^at screenshots (soon...)

##Northligt Tool screenshots
<img src="/readme_assets/NorthlightTool_AW.png"/> <img src="/readme_assets/NorthlightTool_AWAN.png"/>
<img src="/readme_assets/NorthlightTool_AWRem.png"/> <img src="/readme_assets/NorthlightTool_QB.png"/>
<img src="/readme_assets/NorthlightTool_Ctrl.png"/> <img src="/readme_assets/NorthlightTool_about.png"/>
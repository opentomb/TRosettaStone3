TRosettaStone 3
---------------
*Tomb Raider 1-5 file format and engine documentation*

**TRosettaStone 3** (TRS3) is a third iteration of well-known document describing classic Tomb Raider file formats.
It will include all the information from old TRosettaStone from 1999, updated (second) version by Popov, TR5 file format notes by Roy, cutseq.pak file format by sapper, and many other sources. Some information, like function and variable names, is borrowed from leaked TR5 SDK and debug mappings of TR1 beta.

While original TRosettaStone versions were primarily targeted on describing level file structures, third iteration also tries to describe engine behaviour as well.

Documentation project is developed in sync with open-source Tomb Raider engine implementations, like OpenLara and OpenTomb. Therefore, all recent discoveries which appear in source code of these projects are eventually integrated into TRS3 as well.

### Compiling ###

On Windows:

. Install MSYS2 from here: https://www.msys2.org/
. Launch *MSYS2 MSYS* and do `pacman -Syu` and `pacman -Su` commands
. Restart *MSYS2 MSYS* and do `pacman -S python3`, `pacman -S python3-setuptools`, `pacman -S mingw-w64-i686-asciidoc-py3-git` and `pacman -S mingw-w64-i686-python3-pygments` commands
. Launch *MSYS MINGW32* and compile TRS3 with this command: `asciidoc -bhtml5 -a 'newline=\n' [your_path_to_TRS3]/trosettastone.asc`
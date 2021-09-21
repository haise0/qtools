# qtools

A set of tools for working with flash modems on the Qualcom chipset The set consists of a package of utilities and a set of patched loaders.

`qcommand` is an interactive terminal for entering commands through the command port. Goes to replace the terribly inconvenient revskills. Allows to enter command packets byte-by-byte, edit memory, read and view any flash sector.

`qrmem` is a program for reading a dump of the modem's address space.

`qrflash` is a flash reader. Can read both a range of blocks and sections by a section map.

`qwflash` is a program for recording partition images through the bootloader user partitions mode, similar to QPST.

`qwdirect` is a program for direct writing of flash drive blocks with / without OOB through the controller ports (without the involvement of the bootloader logic).

`qdload` is a program for loading bootloaders. Requires the modem to be in download mode or PBL emergency download mode.

`dload.sh` - a script for switching the modem to download mode and sending the specified bootloader to it.

Modified versions of loaders are required for the programs to work. They are collected in the loaders directory, and the source of the patch lies in cmd_05_write_patched.asm. 

This project is being (probably poorly) translated to English for personal use.

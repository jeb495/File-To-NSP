# File-To-NSP
A file to NSP converter


## Revised by jeb495


## From GBATemp: 

A .nsp (pfs0) is a simple file: a header that describes the files it contains, with said files appended to it, in plaintext.
.nsp is the Switch format for installables, similar to what .cia was to the 3ds.
However installing them is currently impossible, and would require signature patching.

This scripts generates nsp files from whatever you tell it to. Anything goes, as long as it is a file. Even empty ones.

To use it, simply drag the files you wish to repack over the script, then enter a name for your nsp.
Alternativaly, use the command prompt and do: nspBuild.py file1 file2...

If you want to see the result, use hactool (or nstools): hactool -t pfs0 path/to/nsp (--outdir=path/to/directory).
No key is required, as the .nsp isn't encrypted.

This script requires python 3

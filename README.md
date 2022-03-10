This project has been ported to C++, https://github.com/MasonGulu/ibm-cassette-maker here.
This will convert binary and ascii files into a format that can be loaded over the IBM PC's cassette port.

The only requirement should be python 3.

Usage:
asciiwrite.py [ascii file] [tape filename]

This takes in a text file with an ascii basic listing in it, and creates a file that can then be loaded using load.
Known issues:
None.

Usage:
binwrite.py [binary file] [tape filename] [segment] [offset]

This takes in a binary file and converts it to a memory dump file that can be loaded using bload.
Known issues:
* The segment and offset seem to do nothing, so I tend to just set them to 0 0.
* To return from ASM programs simply retf with the stack in the same state it was originally.

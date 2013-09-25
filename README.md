cpvdep
======

Copy Verilog source files and all "included" dependencies.

## Description

The script takes two mandatory arguments. The first is the path name
location of the Verilog file to be copied. The second is the destination
directory into which the files will be copied.

The source file will be processed by first being copied to the destination. It
will then be read and any files that have been added via an 'include' macro will
be recursively searched for and if found, copied and processed.

The end result will be the Verilog file and all its 'included' dependencies
will be copied to the destination directory.

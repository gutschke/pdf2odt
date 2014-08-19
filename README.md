pdf2odt/pdf2ods
===============

This script can convert PDF, PNG and JPG files to either ODT or ODS Open
Document files.

In order to perform the conversion, all input files are first converted to
image files and then included as background images for the ODT and ODS Open
Document files. The Open Document files can then be edited by writing on top of
the image(s).

ODT files have one page style per included background image. When editing the
file, simply write text on top of the background image. But be careful not to
insert any page breaks without first adjusting page styles for the page break.

ODS files have one sheet per background image. Each sheet is set up to have
lots of tiny cells. In order to edit the document, you should select
rectangular regions of these small cells and then merge them into bigger
cells. Once all editable cells have been set up, the remainder of the tiny
cells should be protected.  Afterwards, the document behaves very much like a
"normal" spreadsheet.


Usage
=====

On the command line, specify any number of input files followed by the output
file. The output file format is determined by the file name extension of the
output file, or alternatively by the name of the script or by an optional
command line argument.

All output files are generated in the system's default paper size unless
overridden on the command line.

For more details on how to use the script, run without any arguments and it'll
print usage information.


Prerequisites
=============

awk
bash
coreutils
dc
file
ghostscript
imagemagick
sed
zip

pdf2odt
=======

PDF to ODT and ODS format converter. This script also converts PNG and JPG
files.

On the command line, specify any number of input files followed by the output
file. For more details on how to use the script, run without any arguments
and it'll print usage information.

ODT files use different page styles for each image file. They can be edited by
writing text over the background image, but be careful not to insert any page
breaks without first adjusting page styles.

ODS files have a lot of tiny cells. In order to edit the document, rectangular
regions of cells should be merged. Once all editable cells have been set up,
the remainder of the tiny cells should be protected. Afterwards, the document
behaves very much like a "normal" spreadsheet.

All output files have letter format.


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

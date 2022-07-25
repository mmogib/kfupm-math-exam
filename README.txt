Table of Contents
─────────────────




makedtx v1.2 : a Perl script to help create .dtx and .ins files

Last Modified: 2018-02-19
Author : Nicola Talbot
Files : 
        • makedtx.dtx - documented source file
        • makedtx.ins - installation script


The makedtx bundle is provided to help LaTeX2e developers to write the
code and documentation in separate files, and then combine them into a
single .dtx file for distribution.  It automatically generates the
character table, and also writes the associated installation (.ins)
script.

To extract the code do:

┌────
│ latex makedtx.ins
└────

To extract the documentation do after extracting the code:

┌────
│ latexmk -r latexmkrc.pl
└────

If you don't have latexmk or makeindex, you can also do the following to
have the documentation w/o index:

┌────
│ pdflatex makedtx.dtx
│ pdflatex makedtx.dtx
└────

Read the documentation for installation instructions.

This material is subject to the LaTeX Project Public License.  See
[http://www.ctan.org/tex-archive/help/Catalogue/licenses.lppl.html] for
the details of that license.

[http://theoval.cmp.uea.ac.uk/~nlct/]

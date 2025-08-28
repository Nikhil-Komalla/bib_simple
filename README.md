# bib_simple

Using sed in Linux shell
If you have your references in a file (e.g., bib_closebrack, run this command in terminal:


`` sed -E 's/^\(([0-9]+)\)/[\1]/' bib_closebrack > bib_sqbrack``
OR
``bash bib_format.sh``

* Explanation:

-E enables extended regex.
s/^$$([0-9]+)$$/[\1]/ looks for (number) at the start of a line and replaces with [number].
Output is saved to bib_sqbrack.

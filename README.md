# This is a simple handin template

It has a basic setup and gives a handfull of examples on how to
include graphics, create tables, reference figures and tables, and
provides a list of greek letters.

I compile it with `pdflatex`:
> pdflatex main.tex


# Ipe
Personally I am very fund of [Ipe](http://ipe.otfried.org/) which
is a drawing tool that goes very well with LaTeX. Therefor
I have made a directory called graphics containing a file called
`illustrations.pdf` which can be opened by the Ipen program and
modified to ones needs. Along with that comes a macro called
`illustrate` which takes two arguments a *page* and a *width*. The
page specifies the page in the illustrations.pdf file to include
and the width is how much of the text width to take up (0.6 gives
60% of the page)

> \illustrate{1}{0.6}

# Contributions
Please feel free to contribute if anything is missing or anything
could be done better.


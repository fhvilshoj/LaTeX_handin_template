# This is a simple handin template

It has a basic setup and gives a handfull of examples on how to
include graphics, create tables, reference figures and tables, and
provides a list of greek letters. The content should be pretty self
explaining.

I compile it with `pdflatex`:
> pdflatex main.tex

# Structure #

The structure of the project is presented bellow. The main file is the
`main.tex` file which includes the preamble, and contains the content
of the handin. 

```
├── .gitignore              # File that excludes build files etc.
├── included-section.tex    # Tex file to show that imports is possible
├── main.pdf                # The PDF output file
├── main.tex                # The main Tex file
├── preamble.tex            # The file with all the borring setup stuff
├── README.md               # The file containg this description
└── graphics                # Folder for all the graphics
    ├── cat1.jpg
    ├── cat2.jpg
    └── illustrations.pdf   # PDF with graphics made in Ipe
```

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

The following command loads the first page of the `illustrations.pdf` file
centered with a width of 60% of the textwidth.

> \illustrate{1}{0.6}

This command could be included in a figure:

```
\begin{figure}
	\illustrate{1}{0.6}
	\caption{The caption of the figure}
	\label{fig:label-to-reference}
\end{figure}

```


# Contributions
Please feel free to contribute if anything is missing or anything
could be done better.


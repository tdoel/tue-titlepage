# TU/e title page
A (mostly) corporate identity proof titlepage for TU/e theses in LaTeX.

## Package installation
In any case, you need to download package first.
- Download the GitHub repository (green button that reads ‘Code’ and then the ‘Download ZIP’
option) to a path of your choice. Extract the ZIP with your favourite unzipping tool.
- Alternatively, if you are into that sort of stuff, you may also use the command line:
`git clone https://github.com/tdoel/tue-titlepage.git`

### For new documents
1. Download the package as described above.
2. `main.tex` contains a template that you can use to get started. To get rid of this documentation,
simply delete the line `\input{chapter/documentation}`. The result should be an empty
document with a titlepage where some (but not all!) macros are already in use.

### For existing documents
It may very well be that you want to use this titlepage into an existing document, as finishing touch.
After all, content before formatting, not? Luckily, that is also possible.
1. Download the package as described above.
2. Copy the tu directory (only that one) to you LaTeX project. It should be placed in the same
directory as your main LaTeX-file!
3. Include the package with `\usepackage{tu/e}`. Don’t forget the slash! Optionally, can provide
some options to the \usepackage command.

## Usage
The `tu/e.sty` file provides eleven macros that allow you to specify information for the titlepage. You are
free to only use the macro’s that you want to display, you can simply omit the others. If one of these
macros is not used, nothing is printed (this included whitespace, so the layout will not be disturbed
if you omit data). All macros should be used in the preamble - that is, before `\begin{document}`.

The available macros are:
`\title {...}`
`\subtitle {...}`
`\thesistype {...}`
`\author {...}`
`\idnumber {...}`
`\supervisors {...}`
`\version {...}`
`\citydate {...}`
`\institutioninfo {...}`
`\secondinstitutionlogo [...]{...}`
`\secondinstitutioninfo {...}`

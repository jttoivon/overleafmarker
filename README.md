# overleafmarker (version 0.6)

A LaTeX package, which provides the `\olmshownumber` command.
The command draws a big black box near the edge of the page
at appropriate vertical position
with a number in white in it.

Usage:
Include the package with `\usepackage{overleafmarker}`.
By default it assumes six articles. You can override this
with the `papers` option: `\usepackage[papers=4]{overleafmarker}`
or later with the `\olmsetup{papers=4}` command.

Then on the appropriate page in the document, issue command
`\olmshownumber{1}` to show a large black box near the page edge
with roman numeral I in white. The height of the box is
the height of the page divided by the number of papers in the thesis.
In horizontal direction the box spans from the edge of the page
until the beginning of the marginal paragraph. If this is
not suitable, then for instance change the `\marginparsep` to
change the page layout, or give the width of the box
to the `\olmshownumber` as a parameter. For example:
`\olmshownumber[14mm]{2}`

See `thesis-papers.tex` for an example.

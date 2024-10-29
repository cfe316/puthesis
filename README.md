# Unofficial LaTeX Template for Princeton University PhD theses

This template was first developed by [Jeff Dwoskin](https://www.jeffdwoskin.com/) around 2010,
based off a template provided by the Math department.
I've fixed a bug or two and changed some options to make what I think is a better template.

## Basic features
* Different folders for each chapter
* List of figures, list of tables
* Can easily turn off chapters when you're not actively working on them
* Two modes:
  1. print-ProQuest mode (hyperlinks all in black)
  2. regular mode (hyperlinks with nice colors) for the best-quality PDF
* Attempts to comply with [Mudd Library](https://library.princeton.edu/special-collections/policies/masters-theses-and-phd-dissertations-submission-guidelines) standards
* The document itself, once compiled, attempts to explain some of its features
* Nice bibliography formatting using BibLaTeX
  * No doubling-up on URLs if there is also a DOI link
  * Backreferences
* Cleveref for internal references
  * Even better than `hyperref`'s `\autoref`

# How to compile
The main file is `thesis.tex`.

I always use the `latexmk` command which takes care of the process. If you don't use that:

```
pdflatex thesis.tex
biber thesis
pdflatex thesis.tex
pdflatex thesis.tex
```

Feel free to submit Issues, PRs, etc. Let me know if you have trouble with the template.

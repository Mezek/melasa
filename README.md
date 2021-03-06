MeLaSa
=============

`MeLaSa` &mdash; My LaTeX Samples are supporting style files for LaTeX articles used in the process of writing scientific papers.

The contributors can be found in the file "[AUTHORS](AUTHORS)".

Preview
=======

| ![Screenshot1](./images/article.png) |
|:--:|
| *Article style template* |
| ![Screenshot2](./images/revtex.png) |
| *Revtex style template* |

To unpack the files
===================

Clone the project, unpack the files proceeding with the standard latex command `pdflatex`
```
pdflatex melasa.dtx
```

Files
=====

After unpacking you will find files
```
README.txt            Readme file
melasa.pdf            User documentation (see comment below how to make
                                          complete documentary file)
setArticle.sty        ...
setRevtex.sty         ...
setSlovak.sty         ...
template_article.tex  ...
template_revtex.tex   ...
template_ziadost.tex  ...
```

To make documentation
=====================

Run following commands to produce the file *melasa.pdf* with complete documentation
```
makeindex -s gglo.ist -o melasa.gls melasa.glo
makeindex -s gind.ist -o melasa.ind melasa.idx
pdflatex melasa.dtx
```

Using the files
===============

Move files ending *.sty* and *.tex* to a standard TeX input directory. You can edit *.tex* templates for your purposes.

Bugs and remarks
================

Bugs can be reported via the [Issue Tracker](https://github.com/Mezek/melasa/issues) of Github.

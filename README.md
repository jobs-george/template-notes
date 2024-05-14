# Notes Template

Template for writing notes in latex

# Getting Started

Install latex and check it's on path

```sh
latex -v
#> pdfTeX 3.14...
```

Build notes on Windows with

```sh
~/template> pdflatex --shell-escape main.tex
~/template> bibtex main.aux
~/template> makeindex main.aux
~/template> pdflatex main.tex
```

Build notes on Linux with

```sh
~/template$ latex -shell-escape main.tex
~/template$ bibtex main.aux
~/template$ makeindex main.aux
~/template$ pdflatex -shell-escape main.tex
```

Renders a pdf [here](template/main.pdf).

# Batch

For batch builds on Linux use the convenience script

```sh
bash build.sh <folder-name>
```
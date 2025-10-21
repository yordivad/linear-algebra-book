# Linear Algebra Book

This repository contains the LaTeX source for the Linear Algebra book.

## Build locally (requires TeX Live)

On Windows (PowerShell) with a TeX distribution installed (TeX Live or MiKTeX):

```powershell
cd "c:\research\linear algebra"
latexmk -pdf -interaction=nonstopmode -synctex=1 main.tex
```

On Linux / macOS:

```bash
cd "/path/to/repo"
latexmk -pdf -interaction=nonstopmode -synctex=1 main.tex
```

The GitHub Actions CI builds `main.pdf` on push and attaches it as an artifact.

If you need a more minimal TeX Live installation, install the packages used in the workflow (latexmk, texlive-latex-recommended, texlive-latex-extra, texlive-fonts-recommended, texlive-bibtex-extra, biber).

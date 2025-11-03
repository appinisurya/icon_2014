# Plagiarism Detection using Text Mining — ICON 2014

This repository contains the LaTeX source and compiled PDF for a research paper on **plagiarism detection using text mining**, prepared for ICON 2014. It includes the `.tex` manuscript, bibliography/style files, figures, and artifacts to reproduce the camera-ready PDF.

> Primary contents: LaTeX sources (`colacl06.tex`, styles, logs), figures (`graph*.png`, `clustering.png`), and the compiled paper `icon2014_submission_135.pdf`. :contentReference[oaicite:1]{index=1}

---

## Repository Structure

```

icon_2014/
├─ colacl06.tex            # Main LaTeX source
├─ colacl06.sty            # Style file used by the paper
├─ acl.bst                 # BibTeX style
├─ colacl06.{aux,bbl,blg,log,synctex.gz,dvi}  # Build artifacts
├─ graph.png
├─ graph1.png
├─ graph2.png
├─ clustering.png          # Figures used in the paper
├─ instructions.pdf        # Formatting/instructions (conference)
└─ icon2014_submission_135.pdf   # Compiled PDF

````

---

## Build Instructions

You can recompile the PDF locally if you have a LaTeX toolchain.

### Prerequisites
- TeX Live or MiKTeX (with `pdflatex`, `bibtex`)
- (Optional) `latexmk` for one-command builds

### Quick build (pdflatex + bibtex)
```bash
pdflatex colacl06.tex
bibtex colacl06
pdflatex colacl06.tex
pdflatex colacl06.tex
````

The output `colacl06.pdf` should match or be close to `icon2014_submission_135.pdf` (minor diffs can occur due to TeX versions).

### Using latexmk (recommended)

```bash
latexmk -pdf colacl06.tex
# clean build artifacts:
latexmk -c
```

---

## Abstract (1–2 lines)

This paper explores text-mining techniques for **detecting plagiarism**, comparing document similarity signals and discussing preprocessing and evaluation considerations (exact details are in the PDF).

> For the authoritative description and results, please read the compiled paper: `icon2014_submission_135.pdf`. ([GitHub][1])

---

## How to Cite

If you reference this work, please cite the ICON 2014 paper. If you need a BibTeX entry but don’t have the proceeding metadata handy, you can use this placeholder and update fields as appropriate:

```bibtex
@inproceedings{appini_icon2014_plagiarism,
  author    = {Surya Teja Appini and Co-authors},
  title     = {Plagiarism Detection using Text Mining},
  booktitle = {Proceedings of ICON 2014},
  year      = {2014},
  note      = {See repository for PDF and LaTeX sources}
}
```

---

## Reuse & License

No explicit license file is included. By default, that means **all rights reserved**. If you plan to reuse figures, text, or code from this repo, please open an issue to request permission or add a license as appropriate.

---

## Contact

For questions about the paper or build issues, please open a GitHub issue on this repository.

[1]: https://github.com/appinisurya/icon_2014 "GitHub - appinisurya/icon_2014: Plagiarism detection using text mining"

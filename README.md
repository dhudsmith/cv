# Curriculum vitae

The editable source for D. Hudson Smith's general academic CV is `cv.tex`.
The personal website's CV link points to `cv.pdf` in this repository.

## Build

Use a TeX Live installation with ModernCV, TeX Gyre, Latin Modern,
Font Awesome 5, biblatex, biblatex-nature, logreq, and Biber.

```sh
pdflatex -interaction=nonstopmode -halt-on-error cv.tex
biber cv
pdflatex -interaction=nonstopmode -halt-on-error cv.tex
pdflatex -interaction=nonstopmode -halt-on-error cv.tex
```

Inspect the generated PDF after changes, particularly page breaks in the
funding section. Commit `cv.pdf` together with its source updates so the
website download stays current.

## Bibliographies

- `pubs_ml.bib`: published and accepted machine-learning/applied-research papers.
- `pubs_preprints.bib`: preprints, kept separate from published work.
- `pubs_phys.bib`: physics journal papers.
- `pres_ml.bib` and `pres_phys.bib`: presentations, proceedings, and abstracts.

The November 2026 refresh reconciles the older CV with the personal website's
September 2026 bibliography and primary publication records. Publication
status is explicit: the NeurIPS 2026 Hawkes paper is accepted/to appear,
and the MLHC 2026 ICU paper uses its published PMLR citation rather than a
duplicate preprint entry. No publication-count claim is inferred from these
mixed categories.

Google Scholar profile `H2HVoZiAPOsC` was identified, but Google's
unusual-traffic block prevented a full profile export. This update therefore
uses the discovered publisher and preprint records rather than claiming a
complete Scholar synchronization.

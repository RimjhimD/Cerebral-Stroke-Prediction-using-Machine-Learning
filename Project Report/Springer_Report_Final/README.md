# Machine Learning Final Project — Springer Nature LaTeX Report

**Title:** Machine Learning Final Project on Cerebral Stroke Prediction on an Imbalanced Dataset
**Authors:** MD Nishadul Islam, Tahsin Ahmed, Rimjhim Dey
**Affiliation:** Dept. of CSE, Premier University, Chittagong, Bangladesh

## Contents

| File / Folder       | Purpose                                                 |
|---------------------|---------------------------------------------------------|
| `main.tex`          | The report source. Edit this.                           |
| `main.pdf`          | Pre-compiled PDF (19 pages) — preview without running LaTeX. |
| `sn-jnl.cls`        | Springer Nature journal class (required by `main.tex`). |
| `sn-basic.bst`      | BibTeX style (numbered refs). Unused by default since `main.tex` uses `thebibliography` inline. |
| `figures/`          | 22 figures (PNG), all referenced from `main.tex`.       |
| `user-manual.pdf`   | Official Springer Nature template user manual.          |

## How to compile

### Option 1 — Overleaf (easiest)

1. Zip this folder.
2. Log in to Overleaf → **New Project** → **Upload Project** → drop the zip.
3. Open `main.tex`, click **Recompile**. Output appears in the preview pane.

### Option 2 — Local `pdflatex`

From this folder:

```bash
pdflatex main.tex
pdflatex main.tex   # second pass resolves \ref and \cite
```

Output: `main.pdf`.

Required packages (all in `texlive-latex-recommended` + `texlive-latex-extra`):
`graphicx`, `multirow`, `amsmath`, `amssymb`, `amsfonts`, `amsthm`, `mathrsfs`,
`appendix`, `xcolor`, `textcomp`, `manyfoot`, `booktabs`, `url`, `float`.

## Editing tips

- **Change authors / affiliation** → top of `main.tex`, lines with
  `\author*`, `\author`, `\affil*`.
- **Change title** → the `\title[...]{...}` line (short title in brackets, full title in braces).
- **Abstract / keywords** → the `\abstract{...}` and `\keywords{...}` blocks.
- **Add a figure** → drop PNG into `figures/`, then
  `\begin{figure}[!htbp] \centering \includegraphics[width=0.7\textwidth]{your_fig.png} \caption{...} \label{fig:your} \end{figure}`.
- **Add a reference** → append a `\bibitem{key}` block inside `thebibliography`, then cite with `\cite{key}`.
- **Switch to author-year refs** → change line 6 from
  `\documentclass[pdflatex,sn-basic,Numbered]{sn-jnl}` to
  `\documentclass[pdflatex,sn-basic]{sn-jnl}` (remove `Numbered`).

## Report structure

1. Introduction (incl. Related Work, Contributions)
2. Dataset (source, imbalance, missing values, EDA)
3. Methodology (fit-on-train-only pipeline + pseudocode, encoding, feature selection, candidate models, imbalance treatment, hyperparameter search, threshold tuning)
4. Results (journey table, metrics bar chart, final model, confusion matrix, hyperparameter sensitivity, k-fold CV, CV stability)
5. Discussion
6. Conclusion and Future Work
7. References (15 entries)

## Headline numbers

- Test ROC-AUC: **0.8181**
- Test F1 (stroke class): **0.1188**
- Test recall (stroke class): **29.94%** (47/157 caught)
- Test precision (stroke class): **7.41%**
- Threshold (val-tuned): **0.527**
- Final model: shallow class-balanced Random Forest (`n_estimators=201`, `max_depth=5`, `class_weight='balanced'`) trained on SMOTE-augmented training data.

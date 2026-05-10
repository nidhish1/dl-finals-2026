# Pixels to Predictions — Submission

**Report (PDF):** [https://github.com/nidhish1/dl-finals-2026/blob/main/docs/final_report.pdf](https://github.com/nidhish1/dl-finals-2026/blob/main/docs/final_report.pdf)

**Competition:** [Pixels to Predictions — DL Vision Challenge](https://www.kaggle.com/competitions/pixels-to-predictions) (visual question answering with multiple-choice answers).

Training, inference, and submission generation are implemented in `pixels-to-predictions.ipynb`.

> **The notebook is fully reproducible on Kaggle** — [open the pinned notebook here](https://www.kaggle.com/code/dheerajp1728/notebookb7b9ba9957/input?scriptVersionId=317955612).

## Outputs

Artifacts from the pinned run (LoRA adapters, full model export zip, and submission CSVs) are on the notebook **Output** tab for script version `317955612`:

- **LoRA adapters:** [https://www.kaggle.com/code/dheerajp1728/notebookb7b9ba9957/output?scriptVersionId=317955612](https://www.kaggle.com/code/dheerajp1728/notebookb7b9ba9957/output?scriptVersionId=317955612)
- **Full model (bundle / zip):** [https://www.kaggle.com/code/dheerajp1728/notebookb7b9ba9957/output?scriptVersionId=317955612](https://www.kaggle.com/code/dheerajp1728/notebookb7b9ba9957/output?scriptVersionId=317955612)

Both links open the same output page; pick the adapter folder or full model archive from that commit’s file list.

## Repository layout

```
dl-finals-2026/
├── README.md                      # overview, links, reproducibility (this file)
├── docs/
│   └── final_report.pdf           # written report (see link under title)
├── data-exploration.ipynb         # exploratory analysis only
└── pixels-to-predictions.ipynb    # train, infer, submission CSV (matches Kaggle)
```

- **`README.md`** — Competition summary, report/output links, reproducibility callout, and this layout.
- **`docs/final_report.pdf`** — Full write-up (same PDF linked at the top of this README).
- **`data-exploration.ipynb`** — Exploratory data analysis only (distributions, images, labels, notes); no training or `submission.csv`.
- **`pixels-to-predictions.ipynb`** — Same workflow as the pinned Kaggle notebook: SmolVLM + LoRA fine-tuning, validation, optional test-time augmentation (TTA), and export of `submission.csv` (plus other outputs when run on Kaggle).

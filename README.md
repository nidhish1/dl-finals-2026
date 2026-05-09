# Pixels to Predictions — Submission

**Report (PDF):** [https://github.com/nidhish1/dl-finals-2026/blob/main/docs/final_report.pdf](https://github.com/nidhish1/dl-finals-2026/blob/main/docs/final_report.pdf)

**Competition:** [Pixels to Predictions — DL Vision Challenge](https://www.kaggle.com/competitions/pixels-to-predictions) (visual question answering with multiple-choice answers).

Training, inference, and submission generation are implemented in a single Kaggle notebook: `pixels-to-predictions.ipynb`. The notebook is fully reproducible on Kaggle [here](https://www.kaggle.com/code/nidhish1010/pixels-to-predictions/notebook?scriptVersionId=317753258).

## Outputs

Artifacts from the pinned run (LoRA adapters, bundled model export, and submission CSVs) are available on the notebook **Output** tab for script version `317753258`:

- **LoRA adapters:** [https://www.kaggle.com/code/nidhish1010/pixels-to-predictions/output?scriptVersionId=317753258](https://www.kaggle.com/code/nidhish1010/pixels-to-predictions/output?scriptVersionId=317753258)
- **Model bundle (zip / working outputs):** [https://www.kaggle.com/code/nidhish1010/pixels-to-predictions/output?scriptVersionId=317753258](https://www.kaggle.com/code/nidhish1010/pixels-to-predictions/output?scriptVersionId=317753258)

Both links open the same output page; download the files you need from that commit’s output list.

## Repository layout

```
dl-finals-2026/
├── README.md                      # submission overview & links (this file)
├── data-exploration.ipynb         # exploratory analysis only
└── pixels-to-predictions.ipynb    # train, infer, submission CSV (matches Kaggle)
```

- **`README.md`** — Competition summary, reproducibility link, output links, and repository layout.
- **`data-exploration.ipynb`** — Exploratory data analysis only (distributions, images, labels, notes); no training or `submission.csv`.
- **`pixels-to-predictions.ipynb`** — Same workflow as the pinned Kaggle notebook: SmolVLM + LoRA fine-tuning, validation, optional test-time augmentation (TTA), and export of `submission.csv` (plus other outputs when run on Kaggle).

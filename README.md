# NAT-SLN Metastasis Prediction

Code repository for predicting sentinel lymph node (SLN) metastasis after neoadjuvant therapy (NAT) using ultrasound imaging and clinical predictors.


## Planned components

- **Imaging:** Pre- and post-NAT lesion ultrasound model; SLN grayscale, PCEUS, and IVCEUS models; multimodal imaging fusion.
- **Clinical:** Univariate and multivariable logistic regression with selected clinical predictors, represented as a nomogram.
- **Nomograms:** Lesion + SLN, clinical + lesion, clinical + SLN, and clinical + combined imaging probability models.
- **Evaluation:** Discrimination, calibration, decision curve analysis, and classification metrics.

## Repository layout

| Directory | Purpose |
| --- | --- |
| `configs/` | Model and experiment configuration |
| `data/` | Data-loading, ROI preprocessing, and split utilities (no patient data) |
| `models/` | Neural network architectures |
| `training/` | Model training and inference scripts |
| `clinical/` | Clinical logistic regression analysis |
| `nomogram/` | R scripts for clinical and combined nomograms |
| `evaluation/` | Performance evaluation and statistical analyses |
| `scripts/` | Reproduction pipeline entry points |
| `docs/` | Methodology, reconstruction notes, and data dictionary |
| `examples/` | Synthetic or explicitly approved example data only |
| `tests/` | Reproducibility and regression tests |

## Data availability and privacy

Patient-level clinical spreadsheets, original ultrasound images, ROI annotations, patient identifiers, linkage tables, and any unapproved model weights are **not included**. Do not commit them to this repository. The public availability of de-identified data requires a separate privacy, ethics, and institutional review.

## Reproduction status

Original architecture, training settings, preprocessing, probability generation, logistic-regression coefficients, and nomogram scripts must be verified against original source files and checkpoints before claiming reproduction.

## Citation

Citation information will be added after confirmation of the manuscript details.

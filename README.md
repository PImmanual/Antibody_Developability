# Antibody Developability Prediction

Independent computational research project investigating whether antibody sequence-derived and protein-language-model features can be used to predict experimentally measured developability attributes.

## Workflow

1. Construct a developability label from experimentally measured assay attributes.
2. Remove metadata, sequence, assay and derived-label columns to reduce label leakage.
3. Perform L1-regularised logistic regression (LASSO) feature selection.
4. Evaluate selected features using L2-regularised logistic regression.
5. Train a LightGBM classifier using the selected feature set.
6. Use SHAP to inspect model feature contributions.

## Repository contents

- `notebooks/antibody_developability_analysis.ipynb` - cleaned analysis notebook.
- `data/README.md` - input-data requirements and redistribution note.
- `results/README.md` - description of generated outputs.
- `requirements.txt` - Python dependencies.
- `.gitignore` - prevents local datasets and model outputs from being committed accidentally.

## Data

The original antibody dataset is **not included**. The repository contains no experimental dataset, proprietary spreadsheet, or model output derived from the private dataset.

The notebook expects the required input to be supplied locally under `data/`. See `data/README.md` for the expected filenames.

## Reproducibility

The notebook preserves the main modelling workflow used during the project, but the original dataset is required to execute it. Because the data are not distributed with this repository, a fresh clone cannot reproduce the numerical results without authorised access to the input data.

Run the notebook from the `notebooks/` directory so that the repository-relative paths resolve correctly.

## Interpretation

This was an exploratory independent research project, not a production or clinically validated developability model. Model performance should be interpreted in the context of the dataset size, label construction, feature-selection strategy and validation design.

# Antibody Developability Prediction

Independent computational project investigating whether antibody sequence-derived and protein-language-model features can be used to predict experimentally measured developability attributes.

## What is included

- `notebooks/antibody_developability_analysis.ipynb` - cleaned analysis notebook.
- `data/README.md` - notes on the input data.
- `results/README.md` - notes on expected model outputs.
- `requirements.txt` - Python dependencies.

## Analysis workflow

Sequence-derived descriptors and reduced protein-language-model representations were used as candidate features. The workflow included feature cleaning, L1 (LASSO) feature selection, L2 logistic-regression evaluation, and a LightGBM classification workflow. SHAP was used to inspect model feature contributions.

The supplied working notebook also contains earlier experimental/debugging versions of the workflow. Those versions were not reproduced as separate analysis stages here; the repository notebook focuses on the L1/L2 and later LightGBM workflow.

## Data and reproducibility

The original antibody dataset is not included. Do not upload proprietary or restricted data to a public GitHub repository.

The notebook originally used Google Colab/Google Drive paths. These have been replaced with repository-relative paths in the cleaned notebook.

## Important interpretation note

This was an exploratory independent research project. It should not be presented as a production-grade or clinically validated developability model.

# Data

The experimental antibody dataset is not included in this public repository. Do not commit restricted or proprietary data.

For local execution, place the authorised input files in this directory. The supplied notebook references:

- `descriptors_batch_all_merged.csv` for the L1/L2 workflow.
- `descriptors_batch_all_merged_nonzero.csv` for the later LightGBM workflow.

These files are expected to contain the sequence-derived descriptor features and experimentally measured assay columns required by the notebook.

If you do not have permission to redistribute the data, keep the files local and rely on the `.gitignore` rules in the repository.

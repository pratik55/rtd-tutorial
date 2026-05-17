# Module Name: `whifun_functions/whifun_using_other_preproc.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - WHIFUN_USING_OTHER_PREPROC Runs QC on data preprocessed by other software. WHIFUN_USING_OTHER_PREPROC(output_folder) provides a streamlined workflow for performing quality control checks on fMRI data that has been not been preprocessed using WhiFuN. This function guides the user through the process of creating a subject list and then generating a series of quality control plots. It is designed to be a flexible entry point for users who want to leverage the QC capabilities of this toolbox without running the entire preprocessing pipeline. The function performs the following steps: 1. **Create S
  - Internal calls detected: `load_subjects`, `load_subjects_all`, `whifun_check_data`, `whifun_create_Subj_list`, `whifun_plot_data_check_figures`, `whifun_qc`
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_using_other_preproc()`
- **Signature & Definition:** `function whifun_using_other_preproc(output_folder,only_data_check)` (line 1)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_USING_OTHER_PREPROC Runs QC on data preprocessed by other software. WHIFUN_USING_OTHER_PREPROC(output_folder) provides a streamlined workflow for performing quality control checks on fMRI data that has been not been preprocessed using WhiFuN. This function guides the user through the process of creating a subject list and then generating a series of quality control plots. It is designed to be a flexible entry point for users who want to leverage the QC capabilities of this toolbox without running the entire preprocessing pipeline. The function performs the following steps: 1. **Create Subject List**: It calls `whifun_create_Subj_list` to interactively generate a structured subject lis
- **Arguments:**
  - `output_folder` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `only_data_check` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: `load_subjects`, `load_subjects_all`, `whifun_check_data`, `whifun_create_Subj_list`, `whifun_plot_data_check_figures`, `whifun_qc`
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions.

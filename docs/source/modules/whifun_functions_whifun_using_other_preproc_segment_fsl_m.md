# Module Name: `whifun_functions/whifun_using_other_preproc_segment_fsl.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - WHIFUN_USING_OTHER_PREPROC Runs QC on data preprocessed by other software. WHIFUN_USING_OTHER_PREPROC(output_folder) provides a streamlined workflow for performing quality control checks on fMRI data that has been not been preprocessed using WhiFuN. This function guides the user through the process of creating a subject list and then generating a series of quality control plots. It is designed to be a flexible entry point for users who want to leverage the QC capabilities of this toolbox without running the entire preprocessing pipeline. The function performs the following steps: 1. **Create S
  - Internal calls detected: `load_subjects_all`, `my_writetable`, `whifun_check_data`, `whifun_create_file`, `whifun_create_Subj_list`, `whifun_fsl_fast_seg`, `whifun_isnan_or_empty`, `whifun_plot_data_check_figures`, `whifun_qc`, `whifun_smooth_WM_GM_separately_fast`
  - External dependencies detected: MATLAB table/file I/O, FSL command-line suite, Shell/system execution

## `whifun_using_other_preproc_segment_fsl()`

### Syntax
```matlab
function whifun_using_other_preproc_segment_fsl(output_folder,only_data_check)
```
Defined at source line `1`.

### Description
WHIFUN_USING_OTHER_PREPROC Runs QC on data preprocessed by other software. WHIFUN_USING_OTHER_PREPROC(output_folder) provides a streamlined workflow for performing quality control checks on fMRI data that has been not been preprocessed using WhiFuN. This function guides the user through the process of creating a subject list and then generating a series of quality control plots. It is designed to be a flexible entry point for users who want to leverage the QC capabilities of this toolbox without running the entire preprocessing pipeline. The function performs the following steps: 1. **Create Subject List**: It calls `whifun_create_Subj_list` to interactively generate a structured subject lis

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `output_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `only_data_check` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `load_subjects_all`, `my_writetable`, `whifun_check_data`, `whifun_create_file`, `whifun_create_Subj_list`, `whifun_fsl_fast_seg`, `whifun_isnan_or_empty`, `whifun_plot_data_check_figures`, `whifun_qc`, `whifun_smooth_WM_GM_separately_fast`
- **External Dependencies:** MATLAB table/file I/O, FSL command-line suite, Shell/system execution
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects_all`, `my_writetable`, `whifun_check_data`, `whifun_create_file`, `whifun_create_Subj_list`, `whifun_fsl_fast_seg`, `whifun_isnan_or_empty`, `whifun_plot_data_check_figures`, `whifun_qc`, `whifun_smooth_WM_GM_separately_fast`

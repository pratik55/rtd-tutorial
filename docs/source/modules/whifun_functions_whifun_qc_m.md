# Module Name: `whifun_functions/whifun_qc.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - Create input parser
  - Internal calls detected: `whifun_isnan_or_empty`, `whifun_qc_coreg`, `whifun_qc_csf_mask_alignment`, `whifun_qc_filter`, `whifun_qc_final_func_MNI`, `whifun_qc_global_ts`, `whifun_qc_head_motion`, `whifun_qc_initial_align_check`, `whifun_qc_nuisance_regression_global_ts`, `whifun_qc_nuisance_regression_vox_ts`, `whifun_qc_seed_corr`, `whifun_qc_segment`, `whifun_qc_smooth`
  - External dependencies detected: SPM12, SLover/MarsBaR-style visualization helpers

## `whifun_qc()`

### Syntax
```matlab
function whifun_qc(quality_control_path, Subj_list_1, varargin)
```
Defined at source line `1`.

### Description
Create input parser

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `quality_control_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list_1` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Uses explicit parameter parsing or validation. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_isnan_or_empty`, `whifun_qc_coreg`, `whifun_qc_csf_mask_alignment`, `whifun_qc_filter`, `whifun_qc_final_func_MNI`, `whifun_qc_global_ts`, `whifun_qc_head_motion`, `whifun_qc_initial_align_check`, `whifun_qc_nuisance_regression_global_ts`, `whifun_qc_nuisance_regression_vox_ts`, `whifun_qc_seed_corr`, `whifun_qc_segment`, `whifun_qc_smooth`
- **External Dependencies:** SPM12, SLover/MarsBaR-style visualization helpers
- **Called By:** `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`, `whifun_functions/whifun_using_other_preproc.m:1/whifun_using_other_preproc`, `whifun_functions/whifun_using_other_preproc_segment_fsl.m:1/whifun_using_other_preproc_segment_fsl`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_isnan_or_empty`, `whifun_qc_coreg`, `whifun_qc_csf_mask_alignment`, `whifun_qc_filter`, `whifun_qc_final_func_MNI`, `whifun_qc_global_ts`, `whifun_qc_head_motion`, `whifun_qc_initial_align_check`, `whifun_qc_nuisance_regression_global_ts`, `whifun_qc_nuisance_regression_vox_ts`, `whifun_qc_seed_corr`, `whifun_qc_segment`, `whifun_qc_smooth`
- Related callers: `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`, `whifun_functions/whifun_using_other_preproc.m:1/whifun_using_other_preproc`, `whifun_functions/whifun_using_other_preproc_segment_fsl.m:1/whifun_using_other_preproc_segment_fsl`

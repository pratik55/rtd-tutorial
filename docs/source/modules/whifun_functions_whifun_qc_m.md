# Module Name: `whifun_functions/whifun_qc.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - Create input parser
  - Internal calls detected: `whifun_isnan_or_empty`, `whifun_qc_coreg`, `whifun_qc_csf_mask_alignment`, `whifun_qc_filter`, `whifun_qc_final_func_MNI`, `whifun_qc_global_ts`, `whifun_qc_head_motion`, `whifun_qc_initial_align_check`, `whifun_qc_nuisance_regression_global_ts`, `whifun_qc_nuisance_regression_vox_ts`, `whifun_qc_seed_corr`, `whifun_qc_segment`, `whifun_qc_smooth`
  - External dependencies detected: SPM12, SLover/MarsBaR-style visualization helpers

## Function: `whifun_qc()`
- **Signature & Definition:** `function whifun_qc(quality_control_path, Subj_list_1, varargin)` (line 1)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** Create input parser
- **Arguments:**
  - `quality_control_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `Subj_list_1` (structure array containing participant metadata and paths): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: `whifun_isnan_or_empty`, `whifun_qc_coreg`, `whifun_qc_csf_mask_alignment`, `whifun_qc_filter`, `whifun_qc_final_func_MNI`, `whifun_qc_global_ts`, `whifun_qc_head_motion`, `whifun_qc_initial_align_check`, `whifun_qc_nuisance_regression_global_ts`, `whifun_qc_nuisance_regression_vox_ts`, `whifun_qc_seed_corr`, `whifun_qc_segment`, `whifun_qc_smooth`
  - External: SPM12, SLover/MarsBaR-style visualization helpers
  - Called By: `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`, `whifun_functions/whifun_using_other_preproc.m:1/whifun_using_other_preproc`, `whifun_functions/whifun_using_other_preproc_segment_fsl.m:1/whifun_using_other_preproc_segment_fsl`
- **Edge Cases & Exceptions:** Uses explicit parameter parsing or validation. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions.

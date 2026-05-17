# Module Name: `whifun_functions/write_error.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - Display in command
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `write_error()`
- **Signature & Definition:** `function write_error(exception,quality_control_path,name)` (line 1)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** Display in command
- **Arguments:**
  - `exception` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `quality_control_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `name` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_coreg_preproc.m:1/whifun_coreg_preproc`, `whifun_functions/whifun_csf_mask_extraction_preproc.m:1/whifun_csf_mask_extraction_preproc`, `whifun_functions/whifun_discard_initial_volume_preproc.m:1/whifun_discard_initial_volume_preproc`, `whifun_functions/whifun_extract_csf_ts_preproc.m:1/whifun_extract_csf_ts_preproc`, `whifun_functions/whifun_filter_preproc.m:1/whifun_filter_preproc`, `whifun_functions/whifun_get_anat_info.m:1/whifun_get_anat_info`, `whifun_functions/whifun_get_func_info.m:2/whifun_get_func_info`, `whifun_functions/whifun_normalise_preproc.m:1/whifun_normalise_preproc`, `whifun_functions/whifun_nuisance_regress_preproc.m:1/whifun_nuisance_regress_preproc`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`, `whifun_functions/whifun_realignment_preproc.m:1/whifun_realignment_preproc`, `whifun_functions/whifun_segment_preproc.m:1/whifun_segment_preproc`, `whifun_functions/whifun_skull_strip_and_anat_mask_preproc.m:1/whifun_skull_strip_and_anat_mask_preproc`, `whifun_functions/whifun_smooth_preproc.m:1/whifun_smooth_preproc`, `whifun_functions/whifun_smooth_preproc_MNI.m:1/whifun_smooth_preproc_MNI`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

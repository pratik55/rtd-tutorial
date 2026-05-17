# Module Name: `whifun_functions/whifun_post_proc_hcp_dev.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - % ---- input parser ----
  - Internal calls detected: `whifun_discard_initial_volume_preproc`, `whifun_fd_preproc`, `whifun_fsl_fast_seg`, `whifun_isnan_or_empty`, `whifun_smooth_preproc_MNI`
  - External dependencies detected: MATLAB table/file I/O, SPM12, FSL command-line suite

## Function: `whifun_post_proc_hcp_dev()`
- **Signature & Definition:** `function Subj_list_1 = whifun_post_proc_hcp_dev(quality_control_path, Subj_list_1, varargin)` (line 1)
- **Scientific Theory & Formulas:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** % ---- input parser ----
- **Arguments:**
  - `quality_control_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `Subj_list_1` (structure array containing participant metadata and paths): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `Subj_list_1` (structure array containing participant metadata and paths): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `whifun_discard_initial_volume_preproc`, `whifun_fd_preproc`, `whifun_fsl_fast_seg`, `whifun_isnan_or_empty`, `whifun_smooth_preproc_MNI`
  - External: MATLAB table/file I/O, SPM12, FSL command-line suite
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Uses explicit parameter parsing or validation. Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

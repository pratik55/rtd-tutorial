# Module Name: `whifun_functions/whifun_post_proc_hcp_dev.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - % ---- input parser ----
  - Internal calls detected: `whifun_discard_initial_volume_preproc`, `whifun_fd_preproc`, `whifun_fsl_fast_seg`, `whifun_isnan_or_empty`, `whifun_smooth_preproc_MNI`
  - External dependencies detected: MATLAB table/file I/O, SPM12, FSL command-line suite

## `whifun_post_proc_hcp_dev()`

### Syntax
```matlab
function Subj_list_1 = whifun_post_proc_hcp_dev(quality_control_path, Subj_list_1, varargin)
```
Defined at source line `1`.

### Description
% ---- input parser ----

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
#### `Subj_list_1` — structure array containing participant metadata and paths
Output produced by the MATLAB implementation.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Uses explicit parameter parsing or validation. Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_discard_initial_volume_preproc`, `whifun_fd_preproc`, `whifun_fsl_fast_seg`, `whifun_isnan_or_empty`, `whifun_smooth_preproc_MNI`
- **External Dependencies:** MATLAB table/file I/O, SPM12, FSL command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_discard_initial_volume_preproc`, `whifun_fd_preproc`, `whifun_fsl_fast_seg`, `whifun_isnan_or_empty`, `whifun_smooth_preproc_MNI`

# Module Name: `whifun_functions/complete_filepath.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - COMPLETE_FILEPATH Resolves a full file path from segments or wildcards. OUT_PATH = COMPLETE_FILEPATH(DIR, SUBDIR, FILENAME) joins the input segments using the system's file separator and attempts to resolve the final path. If wildcards are used, it returns the first match. INPUTS: varargin - Any number of string or character array segments representing a path (e.g., 'C:', 'Data', 'sub-*_T1w.nii'). OUTPUTS: out_path - A single string of the resolved path. Returns an empty string if the path cannot be found. NOTES: - If multiple files match a wildcard, the function currently returns the folder p
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `complete_filepath()`

### Syntax
```matlab
function out_path = complete_filepath(varargin)
```
Defined at source line `1`.

### Description
COMPLETE_FILEPATH Resolves a full file path from segments or wildcards. OUT_PATH = COMPLETE_FILEPATH(DIR, SUBDIR, FILENAME) joins the input segments using the system's file separator and attempts to resolve the final path. If wildcards are used, it returns the first match. INPUTS: varargin - Any number of string or character array segments representing a path (e.g., 'C:', 'Data', 'sub-*_T1w.nii'). OUTPUTS: out_path - A single string of the resolved path. Returns an empty string if the path cannot be found. NOTES: - If multiple files match a wildcard, the function currently returns the folder path if multiple matches exist, or the full filename if only one match exists. - If the path is not f

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `out_path` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

### More About
Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Uses try/catch; failures are logged, displayed, or returned. Emits warnings for recoverable conditions.

### Algorithms
Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** `Subject_data_folder_details.mlapp:83/SubmitButtonPushed`, `whifun_functions/whifun_check_anat_file.m:1/whifun_check_anat_file`, `whifun_functions/whifun_check_func_file.m:1/whifun_check_func_file`, `whifun_functions/whifun_post_preproc_fmriprep.m:1/whifun_post_preproc_fmriprep`, `whifun_functions/whifun_skullstrip.m:1/whifun_skullstrip`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `Subject_data_folder_details.mlapp:83/SubmitButtonPushed`, `whifun_functions/whifun_check_anat_file.m:1/whifun_check_anat_file`, `whifun_functions/whifun_check_func_file.m:1/whifun_check_func_file`, `whifun_functions/whifun_post_preproc_fmriprep.m:1/whifun_post_preproc_fmriprep`, `whifun_functions/whifun_skullstrip.m:1/whifun_skullstrip`

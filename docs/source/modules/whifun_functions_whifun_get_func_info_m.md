# Module Name: `whifun_functions/whifun_get_func_info.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_GET_FUNC_INFO Extracts information from a functional NIfTI file. [Subj_list_1, voxel_func, n_image] = WHIFUN_GET_FUNC_INFO(now_func_path, Subj_list_1) reads metadata from a functional neuroimaging NIfTI file specified by `now_func_path`. The function updates a subject structure with the extracted information and returns the voxel dimensions and number of time points. This is a core function in a neuroimaging pipeline, as it retrieves critical parameters (like voxel size and number of volumes) that are essential for subsequent preprocessing steps. It handles cases where metadata might be
  - Internal calls detected: `write_error`
  - External dependencies detected: MATLAB NIfTI I/O

## `whifun_get_func_info()`

### Syntax
```matlab
function [Subj_list_1,voxel_func,n_image] = whifun_get_func_info(now_func_path,Subj_list_1,output_folder)
```
Defined at source line `2`.

### Description
WHIFUN_GET_FUNC_INFO Extracts information from a functional NIfTI file. [Subj_list_1, voxel_func, n_image] = WHIFUN_GET_FUNC_INFO(now_func_path, Subj_list_1) reads metadata from a functional neuroimaging NIfTI file specified by `now_func_path`. The function updates a subject structure with the extracted information and returns the voxel dimensions and number of time points. This is a core function in a neuroimaging pipeline, as it retrieves critical parameters (like voxel size and number of volumes) that are essential for subsequent preprocessing steps. It handles cases where metadata might be corrupted or missing. Input Arguments: now_func_path - A `dir` structure (from a call to `dir`) poi

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `now_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list_1` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `output_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Subj_list_1` — structure array containing participant metadata and paths
Output produced by the MATLAB implementation.

#### `voxel_func` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

#### `n_image` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Uses try/catch; failures are logged, displayed, or returned. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `write_error`
- **External Dependencies:** MATLAB NIfTI I/O
- **Called By:** `whifun_functions/whifun_check_data_func.m:1/whifun_check_data_func`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `write_error`
- Related callers: `whifun_functions/whifun_check_data_func.m:1/whifun_check_data_func`

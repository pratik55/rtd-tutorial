# Module Name: `whifun_functions/whifun_get_func_TR.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_GET_FUNC_TR Extracts the TR (Repetition Time) from a functional NIfTI file. [Subj_list_1, tr, report] = WHIFUN_GET_FUNC_TR(now_func_path, Subj_list_1) attempts to read the TR from the header of a functional NIfTI file. The TR is a critical parameter for fMRI data analysis. The function uses `niftiinfo` to access the file's metadata. If the TR is successfully retrieved, it is returned and stored in the subject's structure. In case the TR value is not available, the function sets the TR to `NaN` and generates a report message, which is useful for downstream error handling. Input Arguments
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: MATLAB NIfTI I/O

## `whifun_get_func_TR()`

### Syntax
```matlab
function [Subj_list_1,tr,report] = whifun_get_func_TR(now_func_path,Subj_list_1)
```
Defined at source line `1`.

### Description
WHIFUN_GET_FUNC_TR Extracts the TR (Repetition Time) from a functional NIfTI file. [Subj_list_1, tr, report] = WHIFUN_GET_FUNC_TR(now_func_path, Subj_list_1) attempts to read the TR from the header of a functional NIfTI file. The TR is a critical parameter for fMRI data analysis. The function uses `niftiinfo` to access the file's metadata. If the TR is successfully retrieved, it is returned and stored in the subject's structure. In case the TR value is not available, the function sets the TR to `NaN` and generates a report message, which is useful for downstream error handling. Input Arguments: now_func_path - A `dir` structure (from a call to `dir`) pointing to the functional NIfTI file. Su

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `now_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list_1` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Subj_list_1` — structure array containing participant metadata and paths
Output produced by the MATLAB implementation.

#### `tr` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

#### `report` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Uses try/catch; failures are logged, displayed, or returned. Handles NaN, Inf, or finite-value filtering. Emits warnings for recoverable conditions.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** MATLAB NIfTI I/O
- **Called By:** `whifun_functions/whifun_check_data_func.m:1/whifun_check_data_func`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `whifun_functions/whifun_check_data_func.m:1/whifun_check_data_func`

# Module Name: `whifun_functions/whifun_check_data_func.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CHECK_DATA_FUNC Checks for functional data and extracts its properties. [Subj_list_1, voxel_func, n_image, tr, no_func, report] = WHIFUN_CHECK_DATA_FUNC(...) is a high-level function that orchestrates the process of finding a subject's functional neuroimaging data file, resolving potential ambiguities, and extracting key parameters like voxel size, number of volumes, and TR. The function first calls `whifun_check_func_file` to find the file. If multiple files are found, it sorts them by creation date and selects the oldest one. It then calls `whifun_get_func_info` and `whifun_get_func_T
  - Internal calls detected: `whifun_check_func_file`, `whifun_get_func_info`, `whifun_get_func_TR`
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_check_data_func()`

### Syntax
```matlab
function [Subj_list_1,voxel_func,n_image,tr,no_func,report] = whifun_check_data_func(Subj_list_1,comm_sess_name,func_folder_name,func_data_name,output_folder,report)
```
Defined at source line `1`.

### Description
WHIFUN_CHECK_DATA_FUNC Checks for functional data and extracts its properties. [Subj_list_1, voxel_func, n_image, tr, no_func, report] = WHIFUN_CHECK_DATA_FUNC(...) is a high-level function that orchestrates the process of finding a subject's functional neuroimaging data file, resolving potential ambiguities, and extracting key parameters like voxel size, number of volumes, and TR. The function first calls `whifun_check_func_file` to find the file. If multiple files are found, it sorts them by creation date and selects the oldest one. It then calls `whifun_get_func_info` and `whifun_get_func_TR` to extract the metadata. If no functional data file is found, the function sets a flag (`no_func`

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `Subj_list_1` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `comm_sess_name` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `func_folder_name` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `func_data_name` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `output_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `report` — MATLAB value inferred from source usage
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

#### `tr` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

#### `no_func` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `report` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_check_func_file`, `whifun_get_func_info`, `whifun_get_func_TR`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** `whifun_functions/whifun_check_data.m:1/whifun_check_data`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_check_func_file`, `whifun_get_func_info`, `whifun_get_func_TR`
- Related callers: `whifun_functions/whifun_check_data.m:1/whifun_check_data`

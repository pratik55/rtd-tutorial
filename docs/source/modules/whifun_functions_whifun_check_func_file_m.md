# Module Name: `whifun_functions/whifun_check_func_file.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CHECK_FUNC_FILE Verifies the existence of a functional data file. [now_func_path, report] = WHIFUN_CHECK_FUNC_FILE(Subj_list_1, comm_sess_name, func_folder_name, func_data_name) searches for a functional neuroimaging data file (`.nii` or `.nii.gz`) for a given subject. It constructs the expected file path and checks if the file exists. The function first tries to find the file using the path stored in the subject structure. If that fails, it tries a common alternative with an added '.nii*' extension. If the file is still not found, it generates a detailed error report, including which p
  - Internal calls detected: `complete_filepath`
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_check_func_file()`

### Syntax
```matlab
function [now_func_path,report] = whifun_check_func_file(Subj_list_1,comm_sess_name,func_folder_name,func_data_name)
```
Defined at source line `1`.

### Description
WHIFUN_CHECK_FUNC_FILE Verifies the existence of a functional data file. [now_func_path, report] = WHIFUN_CHECK_FUNC_FILE(Subj_list_1, comm_sess_name, func_folder_name, func_data_name) searches for a functional neuroimaging data file (`.nii` or `.nii.gz`) for a given subject. It constructs the expected file path and checks if the file exists. The function first tries to find the file using the path stored in the subject structure. If that fails, it tries a common alternative with an added '.nii*' extension. If the file is still not found, it generates a detailed error report, including which part of the path (session folder, functional folder, or the file itself) is missing. This function is

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

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `now_func_path` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

#### `report` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `complete_filepath`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** `whifun_functions/whifun_check_data_func.m:1/whifun_check_data_func`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `complete_filepath`
- Related callers: `whifun_functions/whifun_check_data_func.m:1/whifun_check_data_func`

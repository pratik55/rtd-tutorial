# Module Name: `whifun_functions/whifun_isnan_or_empty.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_ISNAN_OR_EMPTY Checks if a specific field in a structure is missing, empty, or NaN. Y = WHIFUN_ISNAN_OR_EMPTY(X, FIELD) This utility function provides a robust check for the existence and validity of a specified field within a MATLAB structure. It is commonly used in programs to validate configuration settings or subject data fields. Input Arguments: X - The input MATLAB structure (struct). FIELD - A character vector or string specifying the name of the field to check (e.g., 'data_path'). Output Arguments: Y - A logical scalar (true or false). Y = true if: 1. The field does not exist in
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_isnan_or_empty()`

### Syntax
```matlab
function y = whifun_isnan_or_empty(x,field)
```
Defined at source line `1`.

### Description
WHIFUN_ISNAN_OR_EMPTY Checks if a specific field in a structure is missing, empty, or NaN. Y = WHIFUN_ISNAN_OR_EMPTY(X, FIELD) This utility function provides a robust check for the existence and validity of a specified field within a MATLAB structure. It is commonly used in programs to validate configuration settings or subject data fields. Input Arguments: X - The input MATLAB structure (struct). FIELD - A character vector or string specifying the name of the field to check (e.g., 'data_path'). Output Arguments: Y - A logical scalar (true or false). Y = true if: 1. The field does not exist in the structure X (as determined by `isfield`). 2. The field exists but its value is an empty array (

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `x` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `field` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `y` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** `whifun_functions/whifun_check_data.m:1/whifun_check_data`, `whifun_functions/whifun_create_qc.m:1/whifun_create_qc`, `whifun_functions/whifun_initialise_manual_motion_error_fields.m:1/whifun_initialise_manual_motion_error_fields`, `whifun_functions/whifun_post_proc_hcp_dev.m:1/whifun_post_proc_hcp_dev`, `whifun_functions/whifun_qc.m:1/whifun_qc`, `whifun_functions/whifun_using_other_preproc_segment_fsl.m:1/whifun_using_other_preproc_segment_fsl`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `whifun_functions/whifun_check_data.m:1/whifun_check_data`, `whifun_functions/whifun_create_qc.m:1/whifun_create_qc`, `whifun_functions/whifun_initialise_manual_motion_error_fields.m:1/whifun_initialise_manual_motion_error_fields`, `whifun_functions/whifun_post_proc_hcp_dev.m:1/whifun_post_proc_hcp_dev`, `whifun_functions/whifun_qc.m:1/whifun_qc`, `whifun_functions/whifun_using_other_preproc_segment_fsl.m:1/whifun_using_other_preproc_segment_fsl`

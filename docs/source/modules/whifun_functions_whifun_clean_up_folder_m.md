# Module Name: `whifun_functions/whifun_clean_up_folder.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CLEAN_UP_FOLDER Compresses all NIfTI (.nii) files in a specified folder into gzipped format (.nii.gz) and removes redundant uncompressed copies. WHIFUN_CLEAN_UP_FOLDER(FOLDER_, LOG_FILE_ID) This utility function performs two main tasks: 1. **Removes Duplicates:** It identifies and deletes any uncompressed NIfTI files (`.nii`) that already have a compressed counterpart (`.<file>.nii.gz`) present in the same folder. 2. **Compresses Remaining Files:** It then compresses all remaining uncompressed `.nii` files into `.nii.gz` format and deletes the original uncompressed `.nii` files. All act
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_clean_up_folder()`

### Syntax
```matlab
function whifun_clean_up_folder(folder_,log_file_id)
```
Defined at source line `1`.

### Description
WHIFUN_CLEAN_UP_FOLDER Compresses all NIfTI (.nii) files in a specified folder into gzipped format (.nii.gz) and removes redundant uncompressed copies. WHIFUN_CLEAN_UP_FOLDER(FOLDER_, LOG_FILE_ID) This utility function performs two main tasks: 1. **Removes Duplicates:** It identifies and deletes any uncompressed NIfTI files (`.nii`) that already have a compressed counterpart (`.<file>.nii.gz`) present in the same folder. 2. **Compresses Remaining Files:** It then compresses all remaining uncompressed `.nii` files into `.nii.gz` format and deletes the original uncompressed `.nii` files. All actions are logged to the specified file handle and the command window. Input Arguments: FOLDER_ - The

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `folder_` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `log_file_id` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** `whifun_functions/whifun_clean_up_after_preprocessing.m:1/whifun_clean_up_after_preprocessing`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `whifun_functions/whifun_clean_up_after_preprocessing.m:1/whifun_clean_up_after_preprocessing`

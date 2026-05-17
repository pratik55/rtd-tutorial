# Module Name: `whifun_functions/whifun_unzip_all_in_folder.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_UNZIP_ALL_IN_FOLDER Unzips all .nii.gz files located directly within a specified folder. WHIFUN_UNZIP_ALL_IN_FOLDER(FOLDER_) This utility function is commonly used in neuroimaging pipelines to decompress gzipped NIfTI files (.nii.gz) into standard NIfTI files (.nii) before processing steps that require the uncompressed format. Input Arguments: FOLDER_ - A character array or string specifying the path to the folder containing the .nii.gz files to be unzipped. Dependencies: MATLAB's built-in `gunzip` and `dir` functions. Author: Pratik Jain
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_unzip_all_in_folder()`

### Syntax
```matlab
function whifun_unzip_all_in_folder(folder_)
```
Defined at source line `1`.

### Description
WHIFUN_UNZIP_ALL_IN_FOLDER Unzips all .nii.gz files located directly within a specified folder. WHIFUN_UNZIP_ALL_IN_FOLDER(FOLDER_) This utility function is commonly used in neuroimaging pipelines to decompress gzipped NIfTI files (.nii.gz) into standard NIfTI files (.nii) before processing steps that require the uncompressed format. Input Arguments: FOLDER_ - A character array or string specifying the path to the folder containing the .nii.gz files to be unzipped. Dependencies: MATLAB's built-in `gunzip` and `dir` functions. Author: Pratik Jain

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `folder_` — character vector or string scalar filesystem path
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
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

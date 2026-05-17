# Module Name: `whifun_functions/whifun_unzip_all_in_folder.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_UNZIP_ALL_IN_FOLDER Unzips all .nii.gz files located directly within a specified folder. WHIFUN_UNZIP_ALL_IN_FOLDER(FOLDER_) This utility function is commonly used in neuroimaging pipelines to decompress gzipped NIfTI files (.nii.gz) into standard NIfTI files (.nii) before processing steps that require the uncompressed format. Input Arguments: FOLDER_ - A character array or string specifying the path to the folder containing the .nii.gz files to be unzipped. Dependencies: MATLAB's built-in `gunzip` and `dir` functions. Author: Pratik Jain
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_unzip_all_in_folder()`
- **Signature & Definition:** `function whifun_unzip_all_in_folder(folder_)` (line 1)
- **Scientific Theory & Formulas:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_UNZIP_ALL_IN_FOLDER Unzips all .nii.gz files located directly within a specified folder. WHIFUN_UNZIP_ALL_IN_FOLDER(FOLDER_) This utility function is commonly used in neuroimaging pipelines to decompress gzipped NIfTI files (.nii.gz) into standard NIfTI files (.nii) before processing steps that require the uncompressed format. Input Arguments: FOLDER_ - A character array or string specifying the path to the folder containing the .nii.gz files to be unzipped. Dependencies: MATLAB's built-in `gunzip` and `dir` functions. Author: Pratik Jain
- **Arguments:**
  - `folder_` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

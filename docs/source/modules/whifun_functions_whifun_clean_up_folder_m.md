# Module Name: `whifun_functions/whifun_clean_up_folder.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CLEAN_UP_FOLDER Compresses all NIfTI (.nii) files in a specified folder into gzipped format (.nii.gz) and removes redundant uncompressed copies. WHIFUN_CLEAN_UP_FOLDER(FOLDER_, LOG_FILE_ID) This utility function performs two main tasks: 1. **Removes Duplicates:** It identifies and deletes any uncompressed NIfTI files (`.nii`) that already have a compressed counterpart (`.<file>.nii.gz`) present in the same folder. 2. **Compresses Remaining Files:** It then compresses all remaining uncompressed `.nii` files into `.nii.gz` format and deletes the original uncompressed `.nii` files. All act
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_clean_up_folder()`
- **Signature & Definition:** `function whifun_clean_up_folder(folder_,log_file_id)` (line 1)
- **Scientific Theory & Formulas:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_CLEAN_UP_FOLDER Compresses all NIfTI (.nii) files in a specified folder into gzipped format (.nii.gz) and removes redundant uncompressed copies. WHIFUN_CLEAN_UP_FOLDER(FOLDER_, LOG_FILE_ID) This utility function performs two main tasks: 1. **Removes Duplicates:** It identifies and deletes any uncompressed NIfTI files (`.nii`) that already have a compressed counterpart (`.<file>.nii.gz`) present in the same folder. 2. **Compresses Remaining Files:** It then compresses all remaining uncompressed `.nii` files into `.nii.gz` format and deletes the original uncompressed `.nii` files. All actions are logged to the specified file handle and the command window. Input Arguments: FOLDER_ - The 
- **Arguments:**
  - `folder_` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `log_file_id` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: `whifun_functions/whifun_clean_up_after_preprocessing.m:1/whifun_clean_up_after_preprocessing`
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

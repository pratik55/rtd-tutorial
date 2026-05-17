# Module Name: `whifun_functions/whifun_gunzip_preproc.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_GUNZIP_PREPROC Unzips .nii.gz files for preprocessing. [Subj_list_1, out_path] = WHIFUN_GUNZIP_PREPROC(now_file_path, Subj_list_1, anat_func) unzips a compressed neuroimaging file (e.g., `file.nii.gz`) to a standard NIfTI file (`file.nii`). The function handles both anatomical and functional data, updating the subject structure with the path to the unzipped file. The function first checks for the existence of multiple files and, if found, selects the oldest one. It then checks if the unzipped `.nii` file already exists to avoid redundant processing. If the `.nii.gz` file is present and 
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_gunzip_preproc()`
- **Signature & Definition:** `function [Subj_list_1,out_path] = whifun_gunzip_preproc(now_file_path,Subj_list_1,anat_func)` (line 1)
- **Scientific Theory & Formulas:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_GUNZIP_PREPROC Unzips .nii.gz files for preprocessing. [Subj_list_1, out_path] = WHIFUN_GUNZIP_PREPROC(now_file_path, Subj_list_1, anat_func) unzips a compressed neuroimaging file (e.g., `file.nii.gz`) to a standard NIfTI file (`file.nii`). The function handles both anatomical and functional data, updating the subject structure with the path to the unzipped file. The function first checks for the existence of multiple files and, if found, selects the oldest one. It then checks if the unzipped `.nii` file already exists to avoid redundant processing. If the `.nii.gz` file is present and the `.nii` file is not, it performs the unzipping operation. Input Arguments: now_file_path - A `dir
- **Arguments:**
  - `now_file_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `Subj_list_1` (structure array containing participant metadata and paths): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `anat_func` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `Subj_list_1` (structure array containing participant metadata and paths): Output produced by the MATLAB implementation.
  - `out_path` (character vector or string scalar filesystem path): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: `whifun_functions/whifun_preproc.m:1/whifun_preproc`
- **Edge Cases & Exceptions:** Emits warnings for recoverable conditions. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

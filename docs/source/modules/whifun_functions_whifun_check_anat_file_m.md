# Module Name: `whifun_functions/whifun_check_anat_file.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CHECK_ANAT_FILE Verifies the existence of an anatomical data file. [now_anat_path, report] = WHIFUN_CHECK_ANAT_FILE(Subj_list_1, comm_sess_name, anat_folder_name) searches for an anatomical neuroimaging data file (`.nii` or `.nii.gz`) for a given subject. It constructs the expected file path and checks if the file exists. The function first uses the path information from the subject structure and checks for a NIfTI file with a `.nii*` extension. If the file is not found, it generates a detailed error report, including which part of the path (session folder, anatomical folder, or the fil
  - Internal calls detected: `complete_filepath`
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_check_anat_file()`
- **Signature & Definition:** `function [now_anat_path,report] = whifun_check_anat_file(Subj_list_1,comm_sess_name,anat_folder_name,anat_data_name)` (line 1)
- **Scientific Theory & Formulas:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_CHECK_ANAT_FILE Verifies the existence of an anatomical data file. [now_anat_path, report] = WHIFUN_CHECK_ANAT_FILE(Subj_list_1, comm_sess_name, anat_folder_name) searches for an anatomical neuroimaging data file (`.nii` or `.nii.gz`) for a given subject. It constructs the expected file path and checks if the file exists. The function first uses the path information from the subject structure and checks for a NIfTI file with a `.nii*` extension. If the file is not found, it generates a detailed error report, including which part of the path (session folder, anatomical folder, or the file itself) is missing. This function is essential for robust preprocessing pipelines, ensuring that t
- **Arguments:**
  - `Subj_list_1` (structure array containing participant metadata and paths): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `comm_sess_name` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `anat_folder_name` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `anat_data_name` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `now_anat_path` (character vector or string scalar filesystem path): Output produced by the MATLAB implementation.
  - `report` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `complete_filepath`
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: `whifun_functions/whifun_check_data_anat.m:1/whifun_check_data_anat`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections.

# Module Name: `whifun_functions/whifun_check_data_anat.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CHECK_DATA_ANAT Checks for the existence and retrieves metadata of the anatomical NIfTI file for a single subject. [SUBJ_LIST_1, VOXEL_ANAT, NO_ANAT, REPORT] = WHIFUN_CHECK_DATA_ANAT(SUBJ_LIST_1, COMM_SESS_NAME, ANAT_FOLDER_NAME, ANAT_DATA_NAME, REPORT) This is a helper function for the initial data quality check process. It locates the anatomical file, handles cases where multiple files are found, and records the file's metadata and status. Input Arguments: SUBJ_LIST_1 - A single-element structure from the subject list, containing the subject's name and path information. COMM_SESS_NAME
  - Internal calls detected: `whifun_check_anat_file`, `whifun_get_anat_info`
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_check_data_anat()`
- **Signature & Definition:** `function [Subj_list_1,voxel_anat,no_anat,report] = whifun_check_data_anat(Subj_list_1,comm_sess_name,anat_folder_name,anat_data_name,output_folder,report)` (line 1)
- **Scientific Theory & Formulas:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_CHECK_DATA_ANAT Checks for the existence and retrieves metadata of the anatomical NIfTI file for a single subject. [SUBJ_LIST_1, VOXEL_ANAT, NO_ANAT, REPORT] = WHIFUN_CHECK_DATA_ANAT(SUBJ_LIST_1, COMM_SESS_NAME, ANAT_FOLDER_NAME, ANAT_DATA_NAME, REPORT) This is a helper function for the initial data quality check process. It locates the anatomical file, handles cases where multiple files are found, and records the file's metadata and status. Input Arguments: SUBJ_LIST_1 - A single-element structure from the subject list, containing the subject's name and path information. COMM_SESS_NAME - Common session name/pattern for anatomical data (e.g., 'ses-01'). ANAT_FOLDER_NAME - Name of the 
- **Arguments:**
  - `Subj_list_1` (structure array containing participant metadata and paths): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `comm_sess_name` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `anat_folder_name` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `anat_data_name` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `output_folder` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `report` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `Subj_list_1` (structure array containing participant metadata and paths): Output produced by the MATLAB implementation.
  - `voxel_anat` (numeric scalar or numeric vector): Output produced by the MATLAB implementation.
  - `no_anat` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
  - `report` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `whifun_check_anat_file`, `whifun_get_anat_info`
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: `whifun_functions/whifun_check_data.m:1/whifun_check_data`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions.

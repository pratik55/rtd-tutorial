# Module Name: `whifun_functions/whifun_get_func_info.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_GET_FUNC_INFO Extracts information from a functional NIfTI file. [Subj_list_1, voxel_func, n_image] = WHIFUN_GET_FUNC_INFO(now_func_path, Subj_list_1) reads metadata from a functional neuroimaging NIfTI file specified by `now_func_path`. The function updates a subject structure with the extracted information and returns the voxel dimensions and number of time points. This is a core function in a neuroimaging pipeline, as it retrieves critical parameters (like voxel size and number of volumes) that are essential for subsequent preprocessing steps. It handles cases where metadata might be
  - Internal calls detected: `write_error`
  - External dependencies detected: MATLAB NIfTI I/O

## Function: `whifun_get_func_info()`
- **Signature & Definition:** `function [Subj_list_1,voxel_func,n_image] = whifun_get_func_info(now_func_path,Subj_list_1,output_folder)` (line 2)
- **Scientific Theory & Formulas:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_GET_FUNC_INFO Extracts information from a functional NIfTI file. [Subj_list_1, voxel_func, n_image] = WHIFUN_GET_FUNC_INFO(now_func_path, Subj_list_1) reads metadata from a functional neuroimaging NIfTI file specified by `now_func_path`. The function updates a subject structure with the extracted information and returns the voxel dimensions and number of time points. This is a core function in a neuroimaging pipeline, as it retrieves critical parameters (like voxel size and number of volumes) that are essential for subsequent preprocessing steps. It handles cases where metadata might be corrupted or missing. Input Arguments: now_func_path - A `dir` structure (from a call to `dir`) poi
- **Arguments:**
  - `now_func_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `Subj_list_1` (structure array containing participant metadata and paths): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `output_folder` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `Subj_list_1` (structure array containing participant metadata and paths): Output produced by the MATLAB implementation.
  - `voxel_func` (numeric scalar or numeric vector): Output produced by the MATLAB implementation.
  - `n_image` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `write_error`
  - External: MATLAB NIfTI I/O
  - Called By: `whifun_functions/whifun_check_data_func.m:1/whifun_check_data_func`
- **Edge Cases & Exceptions:** Uses try/catch; failures are logged, displayed, or returned. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

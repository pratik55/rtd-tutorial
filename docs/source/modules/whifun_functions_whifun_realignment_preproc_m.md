# Module Name: `whifun_functions/whifun_realignment_preproc.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_REALIGNMENT_PREPROC Performs motion correction (realignment) on functional data. [Subj_list_1, out_func_path, out_motion_txt_path] = WHIFUN_REALIGNMENT_PREPROC(...) is a high-level function that orchestrates the realignment step of fMRI preprocessing. Realignment corrects for head motion that occurs during a scan. The function first checks for and resolves multiple input files. It then determines the output file path and, based on the `over_write` flag, decides whether to perform the realignment or skip it if the output file already exists. It calls a sub-function `whifun_realignment` t
  - Internal calls detected: `whifun_create_file`, `whifun_multiple_file_found`, `whifun_realignment`, `write_error`
  - External dependencies detected: MATLAB NIfTI I/O

## Function: `whifun_realignment_preproc()`
- **Signature & Definition:** `function [Subj_list_1,out_func_path,out_motion_txt_path] = whifun_realignment_preproc(quality_control_path,Subj_list_1,in_func_path,Realign_pre,log_fileID, over_write)` (line 1)
- **Scientific Theory & Formulas:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_REALIGNMENT_PREPROC Performs motion correction (realignment) on functional data. [Subj_list_1, out_func_path, out_motion_txt_path] = WHIFUN_REALIGNMENT_PREPROC(...) is a high-level function that orchestrates the realignment step of fMRI preprocessing. Realignment corrects for head motion that occurs during a scan. The function first checks for and resolves multiple input files. It then determines the output file path and, based on the `over_write` flag, decides whether to perform the realignment or skip it if the output file already exists. It calls a sub-function `whifun_realignment` to execute the SPM-based realignment. The function updates the subject structure with the paths to th
- **Arguments:**
  - `quality_control_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `Subj_list_1` (structure array containing participant metadata and paths): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `in_func_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `Realign_pre` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `log_fileID` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `over_write` (logical or numeric flag): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `Subj_list_1` (structure array containing participant metadata and paths): Output produced by the MATLAB implementation.
  - `out_func_path` (character vector or string scalar filesystem path): Output produced by the MATLAB implementation.
  - `out_motion_txt_path` (character vector or string scalar filesystem path): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `whifun_create_file`, `whifun_multiple_file_found`, `whifun_realignment`, `write_error`
  - External: MATLAB NIfTI I/O
  - Called By: `whifun_functions/whifun_preproc.m:1/whifun_preproc`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

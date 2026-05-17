# Module Name: `whifun_functions/whifun_realignment_preproc.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_REALIGNMENT_PREPROC Performs motion correction (realignment) on functional data. [Subj_list_1, out_func_path, out_motion_txt_path] = WHIFUN_REALIGNMENT_PREPROC(...) is a high-level function that orchestrates the realignment step of fMRI preprocessing. Realignment corrects for head motion that occurs during a scan. The function first checks for and resolves multiple input files. It then determines the output file path and, based on the `over_write` flag, decides whether to perform the realignment or skip it if the output file already exists. It calls a sub-function `whifun_realignment` t
  - Internal calls detected: `whifun_create_file`, `whifun_multiple_file_found`, `whifun_realignment`, `write_error`
  - External dependencies detected: MATLAB NIfTI I/O

## `whifun_realignment_preproc()`

### Syntax
```matlab
function [Subj_list_1,out_func_path,out_motion_txt_path] = whifun_realignment_preproc(quality_control_path,Subj_list_1,in_func_path,Realign_pre,log_fileID, over_write)
```
Defined at source line `1`.

### Description
WHIFUN_REALIGNMENT_PREPROC Performs motion correction (realignment) on functional data. [Subj_list_1, out_func_path, out_motion_txt_path] = WHIFUN_REALIGNMENT_PREPROC(...) is a high-level function that orchestrates the realignment step of fMRI preprocessing. Realignment corrects for head motion that occurs during a scan. The function first checks for and resolves multiple input files. It then determines the output file path and, based on the `over_write` flag, decides whether to perform the realignment or skip it if the output file already exists. It calls a sub-function `whifun_realignment` to execute the SPM-based realignment. The function updates the subject structure with the paths to th

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `quality_control_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list_1` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `in_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Realign_pre` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `log_fileID` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `over_write` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Subj_list_1` — structure array containing participant metadata and paths
Output produced by the MATLAB implementation.

#### `out_func_path` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

#### `out_motion_txt_path` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

### More About
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_create_file`, `whifun_multiple_file_found`, `whifun_realignment`, `write_error`
- **External Dependencies:** MATLAB NIfTI I/O
- **Called By:** `whifun_functions/whifun_preproc.m:1/whifun_preproc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_create_file`, `whifun_multiple_file_found`, `whifun_realignment`, `write_error`
- Related callers: `whifun_functions/whifun_preproc.m:1/whifun_preproc`

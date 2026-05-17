# Module Name: `whifun_functions/whifun_get_ts_from_mask.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_GET_TS_FROM_MASK Extracts time series data for each subject from voxels defined by a specified NIfTI mask file. [MASK_ANALYSIS_FOLDER_PATH, MASK_SUBJ_TS_FOLDER, MASK_NAME] = WHIFUN_GET_TS_FROM_MASK(OUT_ANALYSIS_PATH, MASK_PATH, SUBJ_LIST, RESAMPLE_MASK, OVER_WRITE, ...) This function prepares an analysis folder structure, optionally resamples the input mask, and then iterates through all subjects to extract the functional time series for the voxels defined by the mask. Input Arguments: OUT_ANALYSIS_PATH - The root directory where all analysis results for the entire study will be stored.
  - Internal calls detected: `reslice_data`, `whifun_create_file`, `whifun_niftiread`, `y_Read`
  - External dependencies detected: MATLAB NIfTI I/O, MATLAB table/file I/O

## `whifun_get_ts_from_mask()`

### Syntax
```matlab
function [mask_analysis_folder_path,mask_subj_ts_folder,mask_name] = whifun_get_ts_from_mask(out_analysis_path,mask_path,Subj_list,resample_mask,over_write,d_flag,d,steps_,tot_steps)
```
Defined at source line `1`.

### Description
WHIFUN_GET_TS_FROM_MASK Extracts time series data for each subject from voxels defined by a specified NIfTI mask file. [MASK_ANALYSIS_FOLDER_PATH, MASK_SUBJ_TS_FOLDER, MASK_NAME] = WHIFUN_GET_TS_FROM_MASK(OUT_ANALYSIS_PATH, MASK_PATH, SUBJ_LIST, RESAMPLE_MASK, OVER_WRITE, ...) This function prepares an analysis folder structure, optionally resamples the input mask, and then iterates through all subjects to extract the functional time series for the voxels defined by the mask. Input Arguments: OUT_ANALYSIS_PATH - The root directory where all analysis results for the entire study will be stored. MASK_PATH - Full path to the NIfTI file used as the mask (e.g., an ROI or atlas). SUBJ_LIST - Struc

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `out_analysis_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `mask_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `resample_mask` — numeric image/header data, commonly X x Y x Z or X x Y x Z x T
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `over_write` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `d_flag` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `d` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `steps_` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `tot_steps` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `mask_analysis_folder_path` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

#### `mask_subj_ts_folder` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

#### `mask_name` — numeric image/header data, commonly X x Y x Z or X x Y x Z x T
Output produced by the MATLAB implementation.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `reslice_data`, `whifun_create_file`, `whifun_niftiread`, `y_Read`
- **External Dependencies:** MATLAB NIfTI I/O, MATLAB table/file I/O
- **Called By:** `whifun_functions/whifun_create_FN_Kmeans.m:1/whifun_create_FN_Kmeans`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `reslice_data`, `whifun_create_file`, `whifun_niftiread`, `y_Read`
- Related callers: `whifun_functions/whifun_create_FN_Kmeans.m:1/whifun_create_FN_Kmeans`

# Module Name: `whifun_functions/whifun_create_avg_ts.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_GET_AVG_TS Extracts the average time series for each region in a given ROI atlas. AVG_TS_PATH = WHIFUN_GET_AVG_TS(OUT_FOLDER, ROI_PATH, SUBJ_LIST, FIELD, BAND_INFO, QC_PLOTS, OVER_WRITE, D_FLAG, D, STEPS_, TOT_STEPS) This function reads functional MRI data for a list of subjects, resamples the specified Atlas (ROI), and extracts the mean BOLD time series for every non-zero region defined in the Atlas. It also handles optional bandpass filtering and checks for regions with missing functional data. Input Arguments: OUT_FOLDER - Main output directory for saving results and QC plots. ROI_PA
  - Internal calls detected: `functional_connectivity`, `niftisave`, `whifun_create_file`, `whifun_niftiread`
  - External dependencies detected: MATLAB NIfTI I/O, MATLAB table/file I/O, Signal Processing Toolbox, SPM12, ANTs command-line suite

## `whifun_create_avg_ts()`

### Syntax
```matlab
function [avg_ts_path,Subj_list] = whifun_create_avg_ts(out_folder,ROI_path,Subj_list,field,band_info,QC_plots,over_write,d_flag,d,steps_,tot_steps)
```
Defined at source line `1`.

### Description
WHIFUN_GET_AVG_TS Extracts the average time series for each region in a given ROI atlas. AVG_TS_PATH = WHIFUN_GET_AVG_TS(OUT_FOLDER, ROI_PATH, SUBJ_LIST, FIELD, BAND_INFO, QC_PLOTS, OVER_WRITE, D_FLAG, D, STEPS_, TOT_STEPS) This function reads functional MRI data for a list of subjects, resamples the specified Atlas (ROI), and extracts the mean BOLD time series for every non-zero region defined in the Atlas. It also handles optional bandpass filtering and checks for regions with missing functional data. Input Arguments: OUT_FOLDER - Main output directory for saving results and QC plots. ROI_PATH - Full path to the NIfTI file defining the ROI atlas. SUBJ_LIST - (can be created with whifun_cre

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `out_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `ROI_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `field` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `band_info` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `QC_plots` — numeric time-series matrix, commonly T x R, V x T, or T x R x S
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
#### `avg_ts_path` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

#### `Subj_list` — structure array containing participant metadata and paths
Output produced by the MATLAB implementation.

### More About
Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `functional_connectivity`, `niftisave`, `whifun_create_file`, `whifun_niftiread`
- **External Dependencies:** MATLAB NIfTI I/O, MATLAB table/file I/O, Signal Processing Toolbox, SPM12, ANTs command-line suite
- **Called By:** `main.mlapp:1538/ExtractROITImeseriesButtonPushed`, `whifun_functions/whifun_create_FN_Kmeans.m:1/whifun_create_FN_Kmeans`, `whifun_functions/whifun_create_FN_Kmeans_WM_GM.m:1/whifun_create_FN_Kmeans_WM_GM`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `functional_connectivity`, `niftisave`, `whifun_create_file`, `whifun_niftiread`
- Related callers: `main.mlapp:1538/ExtractROITImeseriesButtonPushed`, `whifun_functions/whifun_create_FN_Kmeans.m:1/whifun_create_FN_Kmeans`, `whifun_functions/whifun_create_FN_Kmeans_WM_GM.m:1/whifun_create_FN_Kmeans_WM_GM`

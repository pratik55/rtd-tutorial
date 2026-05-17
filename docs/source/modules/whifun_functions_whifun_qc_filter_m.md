# Module Name: `whifun_functions/whifun_qc_filter.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - WHIFUN_QC_FILTER Generates quality control figures for the filtering step. WHIFUN_QC_FILTER(out_folder, Subj_list_1, over_write, filter_freq_response_flag, filter_lp, filter_hp) creates visual quality control reports to assess the effectiveness of the bandpass filtering applied to functional data. The function performs the following steps: 1. **Check Existence**: It checks if the output plots already exist and, based on the `over_write` flag, either skips or generates new ones. The output includes up to two figures. 2. **Global Time Series Plot**: It plots the mean global time series of the fu
  - Internal calls detected: `whifun_create_file`, `whifun_plot_freqz`
  - External dependencies detected: MATLAB NIfTI I/O, Signal Processing Toolbox

## `whifun_qc_filter()`

### Syntax
```matlab
function whifun_qc_filter(out_folder,Subj_list_1,over_write,filter_freq_response_flag,filter_lp,filter_hp)
```
Defined at source line `1`.

### Description
WHIFUN_QC_FILTER Generates quality control figures for the filtering step. WHIFUN_QC_FILTER(out_folder, Subj_list_1, over_write, filter_freq_response_flag, filter_lp, filter_hp) creates visual quality control reports to assess the effectiveness of the bandpass filtering applied to functional data. The function performs the following steps: 1. **Check Existence**: It checks if the output plots already exist and, based on the `over_write` flag, either skips or generates new ones. The output includes up to two figures. 2. **Global Time Series Plot**: It plots the mean global time series of the functional data *before* and *after* filtering. The global mean is calculated across all voxels at eac

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `out_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list_1` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `over_write` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `filter_freq_response_flag` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `filter_lp` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `filter_hp` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** `whifun_create_file`, `whifun_plot_freqz`
- **External Dependencies:** MATLAB NIfTI I/O, Signal Processing Toolbox
- **Called By:** `whifun_functions/whifun_qc.m:1/whifun_qc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_create_file`, `whifun_plot_freqz`
- Related callers: `whifun_functions/whifun_qc.m:1/whifun_qc`

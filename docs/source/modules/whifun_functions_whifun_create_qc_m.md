# Module Name: `whifun_functions/whifun_create_qc.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - if ~only_check_data %% for subji = 1:length(Subj_list) disp('..') disp(['Currently Processing ' Subj_list(subji).name]) Subj_list_1 = Subj_list(subji); motion_txt = load(complete_filepath(['C:\Users\jainp\Box\practice_NYU_abide\' Subj_list_1.name '\session_1\rest_1\rp_*.txt'])); whifun_qc(quality_control_path,Subj_list_1,'motion_txt',motion_txt); end end
  - Internal calls detected: `whifun_check_data`, `whifun_create_Subj_list`, `whifun_isnan_or_empty`, `whifun_plot_data_check_figures`
  - External dependencies detected: MATLAB table/file I/O

## `whifun_create_qc()`

### Syntax
```matlab
function Subj_list = whifun_create_qc
```
Defined at source line `1`.

### Description
if ~only_check_data %% for subji = 1:length(Subj_list) disp('..') disp(['Currently Processing ' Subj_list(subji).name]) Subj_list_1 = Subj_list(subji); motion_txt = load(complete_filepath(['C:\Users\jainp\Box\practice_NYU_abide\' Subj_list_1.name '\session_1\rest_1\rp_*.txt'])); whifun_qc(quality_control_path,Subj_list_1,'motion_txt',motion_txt); end end

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Subj_list` — structure array containing participant metadata and paths
Output produced by the MATLAB implementation.

### More About
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering.

### Algorithms
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_check_data`, `whifun_create_Subj_list`, `whifun_isnan_or_empty`, `whifun_plot_data_check_figures`
- **External Dependencies:** MATLAB table/file I/O
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_check_data`, `whifun_create_Subj_list`, `whifun_isnan_or_empty`, `whifun_plot_data_check_figures`

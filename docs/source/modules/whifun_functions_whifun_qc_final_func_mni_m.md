# Module Name: `whifun_functions/whifun_qc_final_func_MNI.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - WHIFUN_QC_FINAL_FUNC_MNI Generates final quality control figures for normalized data. WHIFUN_QC_FINAL_FUNC_MNI(out_folder, final_func_MNI, GM_MNI, ..., over_write) creates a suite of visual quality control reports to assess the final preprocessed functional data after it has been normalized to MNI space. The function performs three main checks: 1. **Orthoslice Alignment**: It generates an SPM `check_registration` plot comparing the first volume of the normalized functional image to a standard MNI template. 2. **SLover Alignment**: It uses `whifun_qc_coreg_slover` to create a more detailed over
  - Internal calls detected: `whifun_create_file`, `whifun_qc_coreg_orthoslice`, `whifun_qc_coreg_slover`, `whifun_ts_mask_qc`, `whifun_ts_qc`
  - External dependencies detected: SLover/MarsBaR-style visualization helpers

## `whifun_qc_final_func_MNI()`

### Syntax
```matlab
function whifun_qc_final_func_MNI(out_folder,final_func_MNI,GM_MNI,WM_MNI,CSF_MNI,template_path,motion_txt,name,slover_slices_mni,slover_contour_range_mni,slover_view,over_write)
```
Defined at source line `1`.

### Description
WHIFUN_QC_FINAL_FUNC_MNI Generates final quality control figures for normalized data. WHIFUN_QC_FINAL_FUNC_MNI(out_folder, final_func_MNI, GM_MNI, ..., over_write) creates a suite of visual quality control reports to assess the final preprocessed functional data after it has been normalized to MNI space. The function performs three main checks: 1. **Orthoslice Alignment**: It generates an SPM `check_registration` plot comparing the first volume of the normalized functional image to a standard MNI template. 2. **SLover Alignment**: It uses `whifun_qc_coreg_slover` to create a more detailed overlay plot, which provides a clear visualization of the normalized functional data on the MNI template

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `out_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `final_func_MNI` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `GM_MNI` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `WM_MNI` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `CSF_MNI` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `template_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `motion_txt` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `name` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_slices_mni` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_contour_range_mni` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_view` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `over_write` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_create_file`, `whifun_qc_coreg_orthoslice`, `whifun_qc_coreg_slover`, `whifun_ts_mask_qc`, `whifun_ts_qc`
- **External Dependencies:** SLover/MarsBaR-style visualization helpers
- **Called By:** `whifun_functions/whifun_qc.m:1/whifun_qc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_create_file`, `whifun_qc_coreg_orthoslice`, `whifun_qc_coreg_slover`, `whifun_ts_mask_qc`, `whifun_ts_qc`
- Related callers: `whifun_functions/whifun_qc.m:1/whifun_qc`

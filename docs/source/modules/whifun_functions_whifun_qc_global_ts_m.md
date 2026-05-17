# Module Name: `whifun_functions/whifun_qc_global_ts.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_QC_GLOBAL_TS Generates a quality control figure for global time series. WHIFUN_QC_GLOBAL_TS(out_folder, initial_func, final_func_MNI, motion_txt, func_mask_MNI, name, Reg_, over_write, csf_covariate_path, n_pca, pca_for_temp_reg) creates a visual report to assess the quality of the mean global time series of a subject's functional data. The function plots the mean time series of the original and normalized data, as well as the head motion. The function first checks if the output plot already exists and, based on the `over_write` flag, either skips or generates a new one. It then calls a
  - Internal calls detected: `whifun_create_file`, `whifun_ts_check`
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_qc_global_ts()`

### Syntax
```matlab
function whifun_qc_global_ts(out_folder,initial_func,final_func_MNI,motion_txt,func_mask_MNI,name,Reg_,over_write,csf_covariate_path,n_pca,pca_for_temp_reg)
```
Defined at source line `1`.

### Description
WHIFUN_QC_GLOBAL_TS Generates a quality control figure for global time series. WHIFUN_QC_GLOBAL_TS(out_folder, initial_func, final_func_MNI, motion_txt, func_mask_MNI, name, Reg_, over_write, csf_covariate_path, n_pca, pca_for_temp_reg) creates a visual report to assess the quality of the mean global time series of a subject's functional data. The function plots the mean time series of the original and normalized data, as well as the head motion. The function first checks if the output plot already exists and, based on the `over_write` flag, either skips or generates a new one. It then calls a helper function, `whifun_ts_check` (which is not provided in this file, but is assumed to handle th

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `out_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `initial_func` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `final_func_MNI` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `motion_txt` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `func_mask_MNI` — numeric image/header data, commonly X x Y x Z or X x Y x Z x T
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `name` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Reg_` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `over_write` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `csf_covariate_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `n_pca` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `pca_for_temp_reg` — logical or numeric flag
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
- **Internal Calls:** `whifun_create_file`, `whifun_ts_check`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** `whifun_functions/whifun_qc.m:1/whifun_qc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_create_file`, `whifun_ts_check`
- Related callers: `whifun_functions/whifun_qc.m:1/whifun_qc`

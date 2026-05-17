# Module Name: `whifun_functions/whifun_ts_check.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_TS_CHECK Generates a comprehensive time series quality check figure. WHIFUN_TS_CHECK(func_path_raw, func_path_pro, txt_path, in_anat_mni_mask_path, out_func_mni_mask_path, out_image_path, Reg_, csf_covariate_path, n_pca, pca_for_temp_reg) creates a multi-panel figure to visually inspect the effect of the preprocessing pipeline on a subject's functional time series. The function provides a detailed comparison of data quality before and after key preprocessing steps. The function generates ten plots in a 2x5 grid: - **Global Mean (Raw)**: The mean signal of the raw data. - **Pairwise Vari
  - Internal calls detected: `whifun_calculate_fd`, `whifun_niftiread`
  - External dependencies detected: MATLAB NIfTI I/O, MATLAB table/file I/O, Statistics and Machine Learning Toolbox

## `whifun_ts_check()`

### Syntax
```matlab
function whifun_ts_check(func_path_raw,func_path_pro,txt_path,in_func_mni_mask_path,out_image_path,Reg_,csf_covariate_path,n_pca,pca_for_temp_reg)
```
Defined at source line `1`.

### Description
WHIFUN_TS_CHECK Generates a comprehensive time series quality check figure. WHIFUN_TS_CHECK(func_path_raw, func_path_pro, txt_path, in_anat_mni_mask_path, out_func_mni_mask_path, out_image_path, Reg_, csf_covariate_path, n_pca, pca_for_temp_reg) creates a multi-panel figure to visually inspect the effect of the preprocessing pipeline on a subject's functional time series. The function provides a detailed comparison of data quality before and after key preprocessing steps. The function generates ten plots in a 2x5 grid: - **Global Mean (Raw)**: The mean signal of the raw data. - **Pairwise Variance (Raw)**: A measure of signal change between time points. - **Rigid Body Motion**: The 6 head mo

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `func_path_raw` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `func_path_pro` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `txt_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `in_func_mni_mask_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `out_image_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Reg_` — logical or numeric flag
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
Defines defaults or branches for optional arguments or missing files.

### Algorithms
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_calculate_fd`, `whifun_niftiread`
- **External Dependencies:** MATLAB NIfTI I/O, MATLAB table/file I/O, Statistics and Machine Learning Toolbox
- **Called By:** `whifun_functions/whifun_qc_global_ts.m:1/whifun_qc_global_ts`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_calculate_fd`, `whifun_niftiread`
- Related callers: `whifun_functions/whifun_qc_global_ts.m:1/whifun_qc_global_ts`

## `create_mask()`

### Syntax
```matlab
function mat_mask = create_mask(n)
```
Defined at source line `257`.

### Description
WHIFUN_TS_CHECK Generates a comprehensive time series quality check figure. WHIFUN_TS_CHECK(func_path_raw, func_path_pro, txt_path, in_anat_mni_mask_path, out_func_mni_mask_path, out_image_path, Reg_, csf_covariate_path, n_pca, pca_for_temp_reg) creates a multi-panel figure to visually inspect the effect of the preprocessing pipeline on a subject's functional time series. The function provides a detailed comparison of data quality before and after key preprocessing steps. The function generates ten plots in a 2x5 grid: - **Global Mean (Raw)**: The mean signal of the raw data. - **Pairwise Vari

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `n` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `mat_mask` — numeric image/header data, commonly X x Y x Z or X x Y x Z x T
Output produced by the MATLAB implementation.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

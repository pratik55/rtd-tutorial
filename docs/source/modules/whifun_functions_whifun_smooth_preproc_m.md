# Module Name: `whifun_functions/whifun_smooth_preproc.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_SMOOTH_PREPROC Performs spatial smoothing on functional data. [Subj_list_1, out_func_path] = WHIFUN_SMOOTH_PREPROC(...) is a high-level function that manages the spatial smoothing step of fMRI preprocessing. Smoothing increases the signal-to-noise ratio and allows for inter-subject comparisons. The function supports two types of smoothing: 1. **Separate Smoothing (WM/GM)**: If the `WM_GM` flag is true (1), the function calls `whifun_smooth_WM_GM_separately_fast` to smooth the White Matter and Gray Matter regions independently. This can be beneficial for preserving tissue-specific bounda
  - Internal calls detected: `whifun_create_file`, `whifun_smooth_together`, `whifun_smooth_WM_GM_separately_fast`, `write_error`
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_smooth_preproc()`

### Syntax
```matlab
function [Subj_list_1,out_func_path] = whifun_smooth_preproc(quality_control_path,Subj_list_1,in_func_path,GM_path,WM_path,WM_GM,smooth_fwhm,Smooth_pre,log_fileID,over_write)
```
Defined at source line `1`.

### Description
WHIFUN_SMOOTH_PREPROC Performs spatial smoothing on functional data. [Subj_list_1, out_func_path] = WHIFUN_SMOOTH_PREPROC(...) is a high-level function that manages the spatial smoothing step of fMRI preprocessing. Smoothing increases the signal-to-noise ratio and allows for inter-subject comparisons. The function supports two types of smoothing: 1. **Separate Smoothing (WM/GM)**: If the `WM_GM` flag is true (1), the function calls `whifun_smooth_WM_GM_separately_fast` to smooth the White Matter and Gray Matter regions independently. This can be beneficial for preserving tissue-specific boundaries. 2. **Joint Smoothing**: If `WM_GM` is false (0), the function calls `whifun_smooth_together` t

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `quality_control_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list_1` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `in_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `GM_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `WM_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `WM_GM` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `smooth_fwhm` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Smooth_pre` — logical or numeric flag
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

### More About
Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_create_file`, `whifun_smooth_together`, `whifun_smooth_WM_GM_separately_fast`, `write_error`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** `whifun_functions/whifun_post_preproc_fmriprep.m:1/whifun_post_preproc_fmriprep`, `whifun_functions/whifun_post_proc_hcp.m:1/whifun_post_proc_hcp`, `whifun_functions/whifun_preproc.m:1/whifun_preproc`, `whifun_functions/whifun_preproc_fsl.m:1/whifun_preproc_fsl`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_create_file`, `whifun_smooth_together`, `whifun_smooth_WM_GM_separately_fast`, `write_error`
- Related callers: `whifun_functions/whifun_post_preproc_fmriprep.m:1/whifun_post_preproc_fmriprep`, `whifun_functions/whifun_post_proc_hcp.m:1/whifun_post_proc_hcp`, `whifun_functions/whifun_preproc.m:1/whifun_preproc`, `whifun_functions/whifun_preproc_fsl.m:1/whifun_preproc_fsl`

# Module Name: `whifun_functions/whifun_smooth_WM_GM_separately_fast.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$.
- **Key Features:**
  - loading the data and reslicing the anatomical images to functional resolution
  - Internal calls detected: `niftisave`, `reslice_data`, `whifun_create_file`, `whifun_niftiread`
  - External dependencies detected: MATLAB NIfTI I/O, SPM12, Shell/system execution

## `whifun_smooth_WM_GM_separately_fast()`

### Syntax
```matlab
function [output_gm, output_wm] = whifun_smooth_WM_GM_separately_fast(in_func_path, GM_file_path, WM_file_path ,smooth_pre, gaussian_FWHM, over_write)
```
Defined at source line `1`.

### Description
loading the data and reslicing the anatomical images to functional resolution

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `in_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `GM_file_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `WM_file_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `smooth_pre` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `gaussian_FWHM` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `over_write` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `output_gm` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `output_wm` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `niftisave`, `reslice_data`, `whifun_create_file`, `whifun_niftiread`
- **External Dependencies:** MATLAB NIfTI I/O, SPM12, Shell/system execution
- **Called By:** `whifun_functions/whifun_smooth_preproc.m:1/whifun_smooth_preproc`, `whifun_functions/whifun_using_other_preproc_segment_fsl.m:1/whifun_using_other_preproc_segment_fsl`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `niftisave`, `reslice_data`, `whifun_create_file`, `whifun_niftiread`
- Related callers: `whifun_functions/whifun_smooth_preproc.m:1/whifun_smooth_preproc`, `whifun_functions/whifun_using_other_preproc_segment_fsl.m:1/whifun_using_other_preproc_segment_fsl`

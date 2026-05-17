# Module Name: `whifun_functions/whifun_smooth_together.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_SMOOTH_TOGETHER Performs spatial smoothing on a 4D fMRI volume using SPM's 'smooth' module. OUTPUT = WHIFUN_SMOOTH_TOGETHER(NT, NOW_FUNC_PATH, SMOOTH_FWHM, SMOOTH_PRE) This function sets up and runs an SPM job to apply a Gaussian smoothing kernel to all individual volumes (time points) of a 4D NIfTI file. It prepares the job to run non-interactively and captures the SPM output. Input Arguments: NT - The total number of time points (volumes) in the functional image. NOW_FUNC_PATH - A structure (e.g., from `dir` or `fileparts`) or string containing the path information for the 4D function
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: SPM12, Shell/system execution

## `whifun_smooth_together()`

### Syntax
```matlab
function output = whifun_smooth_together(nt,now_func_path,smooth_fwhm,Smooth_pre)
```
Defined at source line `1`.

### Description
WHIFUN_SMOOTH_TOGETHER Performs spatial smoothing on a 4D fMRI volume using SPM's 'smooth' module. OUTPUT = WHIFUN_SMOOTH_TOGETHER(NT, NOW_FUNC_PATH, SMOOTH_FWHM, SMOOTH_PRE) This function sets up and runs an SPM job to apply a Gaussian smoothing kernel to all individual volumes (time points) of a 4D NIfTI file. It prepares the job to run non-interactively and captures the SPM output. Input Arguments: NT - The total number of time points (volumes) in the functional image. NOW_FUNC_PATH - A structure (e.g., from `dir` or `fileparts`) or string containing the path information for the 4D functional NIfTI file. It must contain the folder and file name for the 4D image. SMOOTH_FWHM - The Full-Wid

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `nt` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `now_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `smooth_fwhm` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Smooth_pre` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `output` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** SPM12, Shell/system execution
- **Called By:** `whifun_functions/whifun_smooth_preproc.m:1/whifun_smooth_preproc`, `whifun_functions/whifun_smooth_preproc_MNI.m:1/whifun_smooth_preproc_MNI`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `whifun_functions/whifun_smooth_preproc.m:1/whifun_smooth_preproc`, `whifun_functions/whifun_smooth_preproc_MNI.m:1/whifun_smooth_preproc_MNI`

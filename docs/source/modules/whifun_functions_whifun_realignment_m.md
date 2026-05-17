# Module Name: `whifun_functions/whifun_realignment.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_REALIGNMENT Performs motion correction (realignment) using SPM. output = WHIFUN_REALIGNMENT(now_func_path, Realign_pre, nt) configures and executes the SPM realignment job to correct for head motion in a time series of functional images. This function creates an SPM batch job to: - **Estimate and Write**: Estimates the motion parameters and applies the transformations to create a new, realigned image series. - **Quality Settings**: Uses a high-quality estimation (`quality = 0.9`), a default separation, and a FWHM smoothing kernel of 5mm. - **Reference Image**: Registers all images to th
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: SPM12, Shell/system execution

## `whifun_realignment()`

### Syntax
```matlab
function output = whifun_realignment(now_func_path,Realign_pre,nt)
```
Defined at source line `1`.

### Description
WHIFUN_REALIGNMENT Performs motion correction (realignment) using SPM. output = WHIFUN_REALIGNMENT(now_func_path, Realign_pre, nt) configures and executes the SPM realignment job to correct for head motion in a time series of functional images. This function creates an SPM batch job to: - **Estimate and Write**: Estimates the motion parameters and applies the transformations to create a new, realigned image series. - **Quality Settings**: Uses a high-quality estimation (`quality = 0.9`), a default separation, and a FWHM smoothing kernel of 5mm. - **Reference Image**: Registers all images to the first image in the series (`rtm = 0`). - **Interpolation**: Uses 2nd-degree B-spline for estimatio

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `now_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Realign_pre` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `nt` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `output` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** SPM12, Shell/system execution
- **Called By:** `whifun_functions/whifun_realignment_preproc.m:1/whifun_realignment_preproc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `whifun_functions/whifun_realignment_preproc.m:1/whifun_realignment_preproc`

# Module Name: `whifun_functions/whifun_ts_extract.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment.
- **Key Features:**
  - WHIFUN_TS_EXTRACT Extracts time series from multiple brain tissue masks. [all_ts, n_gm, n_wm, n_deep_wm, n_csf] = WHIFUN_TS_EXTRACT(...) extracts the time series of all voxels within four predefined brain tissue masks: Gray Matter (GM), Superficial White Matter (WM), Deep White Matter (WM), and Cerebrospinal Fluid (CSF). The function first uses a helper function `whifun_create_mask` to generate binary masks for each tissue type at a specified threshold, resliced to the functional space. It then reads the functional data and extracts the time series for all voxels within each of these masks. Th
  - Internal calls detected: `whifun_niftiread`
  - External dependencies detected: MATLAB NIfTI I/O, SPM12, Shell/system execution

## `whifun_ts_extract()`

### Syntax
```matlab
function [all_ts,n_gm,n_wm,n_deep_wm,n_csf] = whifun_ts_extract(GM_mask_path,WM_mask_path,deep_WM_mask_path,CSF_mask_path,func_path,over_write,thresh_gm,thresh_wm,thresh_deep_wm,thresh_csf)
```
Defined at source line `1`.

### Description
WHIFUN_TS_EXTRACT Extracts time series from multiple brain tissue masks. [all_ts, n_gm, n_wm, n_deep_wm, n_csf] = WHIFUN_TS_EXTRACT(...) extracts the time series of all voxels within four predefined brain tissue masks: Gray Matter (GM), Superficial White Matter (WM), Deep White Matter (WM), and Cerebrospinal Fluid (CSF). The function first uses a helper function `whifun_create_mask` to generate binary masks for each tissue type at a specified threshold, resliced to the functional space. It then reads the functional data and extracts the time series for all voxels within each of these masks. The function separates the WM time series into superficial and deep components, providing more detaile

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `GM_mask_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `WM_mask_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `deep_WM_mask_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `CSF_mask_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `over_write` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `thresh_gm` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `thresh_wm` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `thresh_deep_wm` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `thresh_csf` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `all_ts` — numeric time-series matrix, commonly T x R, V x T, or T x R x S
Output produced by the MATLAB implementation.

#### `n_gm` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `n_wm` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `n_deep_wm` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `n_csf` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_niftiread`
- **External Dependencies:** MATLAB NIfTI I/O
- **Called By:** `whifun_functions/whifun_ts_qc.m:1/whifun_ts_qc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_niftiread`
- Related callers: `whifun_functions/whifun_ts_qc.m:1/whifun_ts_qc`

## `whifun_create_mask()`

### Syntax
```matlab
function output = whifun_create_mask(mask,func_path,thresh_,mask_name)
```
Defined at source line `108`.

### Description
WHIFUN_TS_EXTRACT Extracts time series from multiple brain tissue masks. [all_ts, n_gm, n_wm, n_deep_wm, n_csf] = WHIFUN_TS_EXTRACT(...) extracts the time series of all voxels within four predefined brain tissue masks: Gray Matter (GM), Superficial White Matter (WM), Deep White Matter (WM), and Cerebrospinal Fluid (CSF). The function first uses a helper function `whifun_create_mask` to generate binary masks for each tissue type at a specified threshold, resliced to the functional space. It then reads the functional data and extracts the time series for all voxels within each of these masks. Th

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `mask` — numeric image/header data, commonly X x Y x Z or X x Y x Z x T
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `thresh_` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `mask_name` — numeric image/header data, commonly X x Y x Z or X x Y x Z x T
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `output` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** SPM12, Shell/system execution
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `extract_ts()`

### Syntax
```matlab
function [ts,n] = extract_ts(func_image,mask_path)
```
Defined at source line `159`.

### Description
WHIFUN_TS_EXTRACT Extracts time series from multiple brain tissue masks. [all_ts, n_gm, n_wm, n_deep_wm, n_csf] = WHIFUN_TS_EXTRACT(...) extracts the time series of all voxels within four predefined brain tissue masks: Gray Matter (GM), Superficial White Matter (WM), Deep White Matter (WM), and Cerebrospinal Fluid (CSF). The function first uses a helper function `whifun_create_mask` to generate binary masks for each tissue type at a specified threshold, resliced to the functional space. It then reads the functional data and extracts the time series for all voxels within each of these masks. Th

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `func_image` — numeric image/header data, commonly X x Y x Z or X x Y x Z x T
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `mask_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `ts` — numeric time-series matrix, commonly T x R, V x T, or T x R x S
Output produced by the MATLAB implementation.

#### `n` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_niftiread`
- **External Dependencies:** MATLAB NIfTI I/O
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_niftiread`

## `extract_ts_wm()`

### Syntax
```matlab
function [wm_ts, n_wm, n_deep_wm] = extract_ts_wm(func_image,wm_mask_path,deep_wm_mask_path)
```
Defined at source line `167`.

### Description
WHIFUN_TS_EXTRACT Extracts time series from multiple brain tissue masks. [all_ts, n_gm, n_wm, n_deep_wm, n_csf] = WHIFUN_TS_EXTRACT(...) extracts the time series of all voxels within four predefined brain tissue masks: Gray Matter (GM), Superficial White Matter (WM), Deep White Matter (WM), and Cerebrospinal Fluid (CSF). The function first uses a helper function `whifun_create_mask` to generate binary masks for each tissue type at a specified threshold, resliced to the functional space. It then reads the functional data and extracts the time series for all voxels within each of these masks. Th

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `func_image` — numeric image/header data, commonly X x Y x Z or X x Y x Z x T
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `wm_mask_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `deep_wm_mask_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `wm_ts` — numeric time-series matrix, commonly T x R, V x T, or T x R x S
Output produced by the MATLAB implementation.

#### `n_wm` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `n_deep_wm` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** MATLAB NIfTI I/O
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `create_mask()`

### Syntax
```matlab
function out = create_mask(over_write,func_path,mask_name,thresh_)
```
Defined at source line `180`.

### Description
WHIFUN_TS_EXTRACT Extracts time series from multiple brain tissue masks. [all_ts, n_gm, n_wm, n_deep_wm, n_csf] = WHIFUN_TS_EXTRACT(...) extracts the time series of all voxels within four predefined brain tissue masks: Gray Matter (GM), Superficial White Matter (WM), Deep White Matter (WM), and Cerebrospinal Fluid (CSF). The function first uses a helper function `whifun_create_mask` to generate binary masks for each tissue type at a specified threshold, resliced to the functional space. It then reads the functional data and extracts the time series for all voxels within each of these masks. Th

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `over_write` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `mask_name` — numeric image/header data, commonly X x Y x Z or X x Y x Z x T
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `thresh_` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `out` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

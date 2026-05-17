# Module Name: `whifun_functions/whifun_ts_extract.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment.
- **Key Features:**
  - WHIFUN_TS_EXTRACT Extracts time series from multiple brain tissue masks. [all_ts, n_gm, n_wm, n_deep_wm, n_csf] = WHIFUN_TS_EXTRACT(...) extracts the time series of all voxels within four predefined brain tissue masks: Gray Matter (GM), Superficial White Matter (WM), Deep White Matter (WM), and Cerebrospinal Fluid (CSF). The function first uses a helper function `whifun_create_mask` to generate binary masks for each tissue type at a specified threshold, resliced to the functional space. It then reads the functional data and extracts the time series for all voxels within each of these masks. Th
  - Internal calls detected: `whifun_niftiread`
  - External dependencies detected: MATLAB NIfTI I/O, SPM12, Shell/system execution

## Function: `whifun_ts_extract()`
- **Signature & Definition:** `function [all_ts,n_gm,n_wm,n_deep_wm,n_csf] = whifun_ts_extract(GM_mask_path,WM_mask_path,deep_WM_mask_path,CSF_mask_path,func_path,over_write,thresh_gm,thresh_wm,thresh_deep_wm,thresh_csf)` (line 1)
- **Scientific Theory & Formulas:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_TS_EXTRACT Extracts time series from multiple brain tissue masks. [all_ts, n_gm, n_wm, n_deep_wm, n_csf] = WHIFUN_TS_EXTRACT(...) extracts the time series of all voxels within four predefined brain tissue masks: Gray Matter (GM), Superficial White Matter (WM), Deep White Matter (WM), and Cerebrospinal Fluid (CSF). The function first uses a helper function `whifun_create_mask` to generate binary masks for each tissue type at a specified threshold, resliced to the functional space. It then reads the functional data and extracts the time series for all voxels within each of these masks. The function separates the WM time series into superficial and deep components, providing more detaile
- **Arguments:**
  - `GM_mask_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `WM_mask_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `deep_WM_mask_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `CSF_mask_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `func_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `over_write` (logical or numeric flag): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `thresh_gm` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `thresh_wm` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `thresh_deep_wm` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `thresh_csf` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `all_ts` (numeric time-series matrix, commonly T x R, V x T, or T x R x S): Output produced by the MATLAB implementation.
  - `n_gm` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
  - `n_wm` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
  - `n_deep_wm` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
  - `n_csf` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `whifun_niftiread`
  - External: MATLAB NIfTI I/O
  - Called By: `whifun_functions/whifun_ts_qc.m:1/whifun_ts_qc`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files.

## Function: `whifun_create_mask()`
- **Signature & Definition:** `function output = whifun_create_mask(mask,func_path,thresh_,mask_name)` (line 108)
- **Scientific Theory & Formulas:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_TS_EXTRACT Extracts time series from multiple brain tissue masks. [all_ts, n_gm, n_wm, n_deep_wm, n_csf] = WHIFUN_TS_EXTRACT(...) extracts the time series of all voxels within four predefined brain tissue masks: Gray Matter (GM), Superficial White Matter (WM), Deep White Matter (WM), and Cerebrospinal Fluid (CSF). The function first uses a helper function `whifun_create_mask` to generate binary masks for each tissue type at a specified threshold, resliced to the functional space. It then reads the functional data and extracts the time series for all voxels within each of these masks. Th
- **Arguments:**
  - `mask` (numeric image/header data, commonly X x Y x Z or X x Y x Z x T): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `func_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `thresh_` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `mask_name` (numeric image/header data, commonly X x Y x Z or X x Y x Z x T): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `output` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: SPM12, Shell/system execution
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `extract_ts()`
- **Signature & Definition:** `function [ts,n] = extract_ts(func_image,mask_path)` (line 159)
- **Scientific Theory & Formulas:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_TS_EXTRACT Extracts time series from multiple brain tissue masks. [all_ts, n_gm, n_wm, n_deep_wm, n_csf] = WHIFUN_TS_EXTRACT(...) extracts the time series of all voxels within four predefined brain tissue masks: Gray Matter (GM), Superficial White Matter (WM), Deep White Matter (WM), and Cerebrospinal Fluid (CSF). The function first uses a helper function `whifun_create_mask` to generate binary masks for each tissue type at a specified threshold, resliced to the functional space. It then reads the functional data and extracts the time series for all voxels within each of these masks. Th
- **Arguments:**
  - `func_image` (numeric image/header data, commonly X x Y x Z or X x Y x Z x T): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `mask_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `ts` (numeric time-series matrix, commonly T x R, V x T, or T x R x S): Output produced by the MATLAB implementation.
  - `n` (numeric scalar or numeric vector): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `whifun_niftiread`
  - External: MATLAB NIfTI I/O
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `extract_ts_wm()`
- **Signature & Definition:** `function [wm_ts, n_wm, n_deep_wm] = extract_ts_wm(func_image,wm_mask_path,deep_wm_mask_path)` (line 167)
- **Scientific Theory & Formulas:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_TS_EXTRACT Extracts time series from multiple brain tissue masks. [all_ts, n_gm, n_wm, n_deep_wm, n_csf] = WHIFUN_TS_EXTRACT(...) extracts the time series of all voxels within four predefined brain tissue masks: Gray Matter (GM), Superficial White Matter (WM), Deep White Matter (WM), and Cerebrospinal Fluid (CSF). The function first uses a helper function `whifun_create_mask` to generate binary masks for each tissue type at a specified threshold, resliced to the functional space. It then reads the functional data and extracts the time series for all voxels within each of these masks. Th
- **Arguments:**
  - `func_image` (numeric image/header data, commonly X x Y x Z or X x Y x Z x T): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `wm_mask_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `deep_wm_mask_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `wm_ts` (numeric time-series matrix, commonly T x R, V x T, or T x R x S): Output produced by the MATLAB implementation.
  - `n_wm` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
  - `n_deep_wm` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: MATLAB NIfTI I/O
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `create_mask()`
- **Signature & Definition:** `function out = create_mask(over_write,func_path,mask_name,thresh_)` (line 180)
- **Scientific Theory & Formulas:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_TS_EXTRACT Extracts time series from multiple brain tissue masks. [all_ts, n_gm, n_wm, n_deep_wm, n_csf] = WHIFUN_TS_EXTRACT(...) extracts the time series of all voxels within four predefined brain tissue masks: Gray Matter (GM), Superficial White Matter (WM), Deep White Matter (WM), and Cerebrospinal Fluid (CSF). The function first uses a helper function `whifun_create_mask` to generate binary masks for each tissue type at a specified threshold, resliced to the functional space. It then reads the functional data and extracts the time series for all voxels within each of these masks. Th
- **Arguments:**
  - `over_write` (logical or numeric flag): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `func_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `mask_name` (numeric image/header data, commonly X x Y x Z or X x Y x Z x T): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `thresh_` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `out` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections.

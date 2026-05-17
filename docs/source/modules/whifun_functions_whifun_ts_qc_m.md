# Module Name: `whifun_functions/whifun_ts_qc.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_TS_QC Generates a quality control figure for time series and motion. WHIFUN_TS_QC(GM_mask_path, WM_mask_path, CSF_mask_path, func_path, motion_txt_path, num_erosions, Par_name, over_write, f) creates a comprehensive figure for a single subject, visualizing the time series of key brain tissues alongside framewise displacement (FD). The function first creates a "deep White Matter (WM)" mask by eroding the standard WM mask, which helps to isolate a signal that is less likely to contain a gray matter component. It then extracts the time series from the Gray Matter (GM), Superficial White Ma
  - Internal calls detected: `whifun_calculate_fd`, `whifun_erode`, `whifun_ts_extract`
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_ts_qc()`
- **Signature & Definition:** `function whifun_ts_qc(GM_mask_path,WM_mask_path,CSF_mask_path,func_path,motion_txt_path,num_erosions,Par_name,over_write,f)` (line 1)
- **Scientific Theory & Formulas:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_TS_QC Generates a quality control figure for time series and motion. WHIFUN_TS_QC(GM_mask_path, WM_mask_path, CSF_mask_path, func_path, motion_txt_path, num_erosions, Par_name, over_write, f) creates a comprehensive figure for a single subject, visualizing the time series of key brain tissues alongside framewise displacement (FD). The function first creates a "deep White Matter (WM)" mask by eroding the standard WM mask, which helps to isolate a signal that is less likely to contain a gray matter component. It then extracts the time series from the Gray Matter (GM), Superficial White Matter (WM), Deep White Matter, and Cerebrospinal Fluid (CSF) using a helper function. The generated f
- **Arguments:**
  - `GM_mask_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `WM_mask_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `CSF_mask_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `func_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `motion_txt_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `num_erosions` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `Par_name` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `over_write` (logical or numeric flag): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `f` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: `whifun_calculate_fd`, `whifun_erode`, `whifun_ts_extract`
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: `whifun_functions/whifun_qc_final_func_MNI.m:1/whifun_qc_final_func_MNI`, `whifun_functions/whifun_qc_normalize.m:1/whifun_qc_normalize`, `whifun_functions/whifun_qc_nuisance_regression_vox_ts.m:1/whifun_qc_nuisance_regression_vox_ts`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files.

## Function: `create_mask()`
- **Signature & Definition:** `function out = create_mask(over_write,mask_path,mask_name)` (line 108)
- **Scientific Theory & Formulas:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_TS_QC Generates a quality control figure for time series and motion. WHIFUN_TS_QC(GM_mask_path, WM_mask_path, CSF_mask_path, func_path, motion_txt_path, num_erosions, Par_name, over_write, f) creates a comprehensive figure for a single subject, visualizing the time series of key brain tissues alongside framewise displacement (FD). The function first creates a "deep White Matter (WM)" mask by eroding the standard WM mask, which helps to isolate a signal that is less likely to contain a gray matter component. It then extracts the time series from the Gray Matter (GM), Superficial White Ma
- **Arguments:**
  - `over_write` (logical or numeric flag): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `mask_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `mask_name` (numeric image/header data, commonly X x Y x Z or X x Y x Z x T): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `out` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections.

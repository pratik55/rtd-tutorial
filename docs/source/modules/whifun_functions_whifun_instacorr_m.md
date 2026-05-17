# Module Name: `whifun_functions/whifun_instacorr.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Key Features:**
  - No leading help block was present; behavior was inferred from signatures and static calls.
  - Internal calls detected: `whifun_convert_coords`, `whifun_create_sphere`, `whifun_extract_ts_from_vox`
  - External dependencies detected: MATLAB NIfTI I/O, Statistics and Machine Learning Toolbox

## Function: `whifun_seed_corr()`
- **Signature & Definition:** `function out_map = whifun_seed_corr(func_image_path,seed,radius,mask)` (line 1)
- **Scientific Theory & Formulas:** Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** Routine has no dedicated help block; purpose was inferred from its name, surrounding module, and static call context.
- **Arguments:**
  - `func_image_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `seed` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `radius` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `mask` (numeric image/header data, commonly X x Y x Z or X x Y x Z x T): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `out_map` (numeric scalar, vector, matrix, or multidimensional array): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `whifun_convert_coords`, `whifun_create_sphere`, `whifun_extract_ts_from_vox`
  - External: MATLAB NIfTI I/O, Statistics and Machine Learning Toolbox
  - Called By: `whifun_functions/whifun_seed_corr_qc_plot.m:1/whifun_seed_corr_qc_plot`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering.

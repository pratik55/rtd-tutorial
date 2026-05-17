# Module Name: `whifun_functions/whifun_seed_corr.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_SEED_CORR Performs Seed-Based Functional Connectivity (FC) Analysis. [OUT_MAP, MATLAB_COR, THRESH] = WHIFUN_SEED_CORR(FUNC_IMAGE_PATH, SEED, RADIUS, OUTPUT_PATH, THRESH, MASK) This function calculates the Pearson correlation map between the mean time series of a spherical seed region (defined in MNI coordinates) and the time series of every other voxel in the brain. It saves the resulting correlation map and optionally saves two thresholded maps (positive and negative correlations). Input Arguments: FUNC_IMAGE_PATH - Full path to the 4D NIfTI file of the functional image. SEED - 3-eleme
  - Internal calls detected: `niftisave`, `whifun_convert_coords`, `whifun_create_sphere`, `whifun_extract_ts_from_vox`, `whifun_niftiread`
  - External dependencies detected: MATLAB NIfTI I/O, Statistics and Machine Learning Toolbox

## Function: `whifun_seed_corr()`
- **Signature & Definition:** `function [out_map,matlab_cor,thresh] = whifun_seed_corr(func_image_path,seed,radius,output_path,thresh,mask)` (line 1)
- **Scientific Theory & Formulas:** Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_SEED_CORR Performs Seed-Based Functional Connectivity (FC) Analysis. [OUT_MAP, MATLAB_COR, THRESH] = WHIFUN_SEED_CORR(FUNC_IMAGE_PATH, SEED, RADIUS, OUTPUT_PATH, THRESH, MASK) This function calculates the Pearson correlation map between the mean time series of a spherical seed region (defined in MNI coordinates) and the time series of every other voxel in the brain. It saves the resulting correlation map and optionally saves two thresholded maps (positive and negative correlations). Input Arguments: FUNC_IMAGE_PATH - Full path to the 4D NIfTI file of the functional image. SEED - 3-element vector [x, y, z] in MNI space defining the center of the spherical seed region (e.g., [-4 58 20])
- **Arguments:**
  - `func_image_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `seed` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `radius` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `output_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `thresh` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `mask` (numeric image/header data, commonly X x Y x Z or X x Y x Z x T): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `out_map` (numeric scalar, vector, matrix, or multidimensional array): Output produced by the MATLAB implementation.
  - `matlab_cor` (numeric scalar, vector, matrix, or multidimensional array): Output produced by the MATLAB implementation.
  - `thresh` (numeric scalar or numeric vector): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `niftisave`, `whifun_convert_coords`, `whifun_create_sphere`, `whifun_extract_ts_from_vox`, `whifun_niftiread`
  - External: MATLAB NIfTI I/O, Statistics and Machine Learning Toolbox
  - Called By: `whifun_functions/whifun_seed_corr_qc_plot.m:1/whifun_seed_corr_qc_plot`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Emits warnings for recoverable conditions.

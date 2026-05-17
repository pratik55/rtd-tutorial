# Module Name: `whifun_functions/whifun_create_FN_Kmeans.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CREATE_FN_KMEANS Creates WM/GM Functional Networks using K-means clustering whifun_create_FN_Kmeans(...) performs K-means clustering on the average voxel-level functional connectivity matrix across subjects and generates functional networks (FNs). It also saves BrainNet images and average time series for each FN. Required Inputs: output_folder - Path to output folder WM_or_GM - 'WM' or 'GM' K_range_l - Lower bound for K (clusters) K_range_h - Upper bound for K group_mask_path - Path to group-level brain mask (NIfTI) Optional Inputs: sub_sample_choose- Subsample flag/strategy (default: '
  - Internal calls detected: `load_subjects`, `whifun_build_net`, `whifun_create_avg_ts`, `whifun_create_avg_voxel_level_fc`, `whifun_create_brainnet_images`, `whifun_create_fn_from_parrcorr_and_ttest`, `whifun_get_best_k`, `whifun_get_FN_kmeans`, `whifun_get_ts_from_mask`, `whifun_partial_corr`
  - External dependencies detected: MATLAB NIfTI I/O, ANTs command-line suite, BrainNet Viewer

## `whifun_create_FN_Kmeans()`

### Syntax
```matlab
function whifun_create_FN_Kmeans(output_folder,WM_or_GM,K_range_l,K_range_h,group_mask_path,varargin)
```
Defined at source line `1`.

### Description
WHIFUN_CREATE_FN_KMEANS Creates WM/GM Functional Networks using K-means clustering whifun_create_FN_Kmeans(...) performs K-means clustering on the average voxel-level functional connectivity matrix across subjects and generates functional networks (FNs). It also saves BrainNet images and average time series for each FN. Required Inputs: output_folder - Path to output folder WM_or_GM - 'WM' or 'GM' K_range_l - Lower bound for K (clusters) K_range_h - Upper bound for K group_mask_path - Path to group-level brain mask (NIfTI) Optional Inputs: sub_sample_choose- Subsample flag/strategy (default: 'Sub sample') CV_folds - Number of cross-validation folds (default: 4) focus_check - Apply focus mask

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `output_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `WM_or_GM` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `K_range_l` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `K_range_h` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `group_mask_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Uses explicit parameter parsing or validation. Defines defaults or branches for optional arguments or missing files. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `load_subjects`, `whifun_build_net`, `whifun_create_avg_ts`, `whifun_create_avg_voxel_level_fc`, `whifun_create_brainnet_images`, `whifun_create_fn_from_parrcorr_and_ttest`, `whifun_get_best_k`, `whifun_get_FN_kmeans`, `whifun_get_ts_from_mask`, `whifun_partial_corr`
- **External Dependencies:** MATLAB NIfTI I/O, ANTs command-line suite, BrainNet Viewer
- **Called By:** `main.mlapp:1298/CreateWMFNButtonPushed`, `main.mlapp:1408/CreateGMFNButtonPushed`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects`, `whifun_build_net`, `whifun_create_avg_ts`, `whifun_create_avg_voxel_level_fc`, `whifun_create_brainnet_images`, `whifun_create_fn_from_parrcorr_and_ttest`, `whifun_get_best_k`, `whifun_get_FN_kmeans`, `whifun_get_ts_from_mask`, `whifun_partial_corr`
- Related callers: `main.mlapp:1298/CreateWMFNButtonPushed`, `main.mlapp:1408/CreateGMFNButtonPushed`

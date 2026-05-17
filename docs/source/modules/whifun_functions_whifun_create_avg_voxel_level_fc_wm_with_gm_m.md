# Module Name: `whifun_functions/whifun_create_avg_voxel_level_fc_WM_with_GM.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CREATE_AVG_VOXEL_LEVEL_FC Creates the group-average Voxel-Level Functional Connectivity (FC) matrix. [AVG_VOX_LEVEL_FC, GROUP_MASK_VOXELS] = WHIFUN_CREATE_AVG_VOXEL_LEVEL_FC(CLUSTER_FOLDER, SUBJ_LIST, GROUP_MASK_PATH, SUB_SAMPLE_CHOOSE, WM_OR_GM, FOCUS_REGION_CHECK, FOCUS_REGION_MASK_PATH, OVER_WRITE, ...) This function computes the group-average FC matrix between all voxels in a target mask (e.g., WM or GM) and either all or a subsampled subset of those voxels. This average matrix is then used as the input feature matrix for group-level clustering. The function includes memory checks a
  - Internal calls detected: `reslice_data`, `whifun_create_file`
  - External dependencies detected: MATLAB NIfTI I/O, MATLAB table/file I/O, Statistics and Machine Learning Toolbox, ANTs command-line suite

## `whifun_create_avg_voxel_level_fc_WM_with_GM()`

### Syntax
```matlab
function [avg_vox_level_FC,wm_group_mask_voxels] = whifun_create_avg_voxel_level_fc_WM_with_GM(cluster_folder,Subj_list,wm_group_mask_path,gm_group_mask_path,sub_sample_choose,over_write,d_flag,d,steps_,tot_steps)
```
Defined at source line `1`.

### Description
WHIFUN_CREATE_AVG_VOXEL_LEVEL_FC Creates the group-average Voxel-Level Functional Connectivity (FC) matrix. [AVG_VOX_LEVEL_FC, GROUP_MASK_VOXELS] = WHIFUN_CREATE_AVG_VOXEL_LEVEL_FC(CLUSTER_FOLDER, SUBJ_LIST, GROUP_MASK_PATH, SUB_SAMPLE_CHOOSE, WM_OR_GM, FOCUS_REGION_CHECK, FOCUS_REGION_MASK_PATH, OVER_WRITE, ...) This function computes the group-average FC matrix between all voxels in a target mask (e.g., WM or GM) and either all or a subsampled subset of those voxels. This average matrix is then used as the input feature matrix for group-level clustering. The function includes memory checks and handles individual subject-specific segmentation masks. Input Arguments: CLUSTER_FOLDER - Output

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `cluster_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `wm_group_mask_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `gm_group_mask_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `sub_sample_choose` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `over_write` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `d_flag` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `d` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `steps_` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `tot_steps` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `avg_vox_level_FC` — numeric scalar, vector, matrix, or multidimensional array
Output produced by the MATLAB implementation.

#### `wm_group_mask_voxels` — numeric image/header data, commonly X x Y x Z or X x Y x Z x T
Output produced by the MATLAB implementation.

### More About
Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands. May pause for interactive user input, which affects batch reproducibility.

### Algorithms
Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `reslice_data`, `whifun_create_file`
- **External Dependencies:** MATLAB NIfTI I/O, MATLAB table/file I/O, Statistics and Machine Learning Toolbox, ANTs command-line suite
- **Called By:** `whifun_functions/whifun_create_FN_Kmeans_WM_GM.m:1/whifun_create_FN_Kmeans_WM_GM`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `reslice_data`, `whifun_create_file`
- Related callers: `whifun_functions/whifun_create_FN_Kmeans_WM_GM.m:1/whifun_create_FN_Kmeans_WM_GM`

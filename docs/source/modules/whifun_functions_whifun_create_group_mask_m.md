# Module Name: `whifun_functions/whifun_create_group_mask.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CREATE_GROUP_MASK Creates group-level White Matter (WM) and Gray Matter (GM) masks. [GROUP_MASK_WM_PATH, GROUP_MASK_GM_PATH, D] = WHIFUN_CREATE_GROUP_MASK(OUT_ANALYSIS_PATH, SUBJ_LIST, GRP_WM_MASK_NAME, INDI_THRES_WM, GRP_THRES_WM, GRP_GM_MASK_NAME, INDI_THRES_GM, GRP_THRES_GM, OVER_WRITE, D_FLAG, D, STEPS_, TOT_STEPS) This function creates group-level WM and GM masks based on individual segmentation maps (e.g., from SPM/CAT) and functional data coverage. Input Arguments: OUT_ANALYSIS_PATH - Main output directory where 'Group_Masks' folder will be created. SUBJ_LIST - Structure array co
  - Internal calls detected: `niftisave`, `reslice_data`, `whifun_create_file`
  - External dependencies detected: MATLAB NIfTI I/O, ANTs command-line suite, BrainNet Viewer

## `whifun_create_group_mask()`

### Syntax
```matlab
function [group_mask_WM_path,group_mask_GM_path,d] = whifun_create_group_mask(out_analysis_path,Subj_list,grp_WM_mask_name,indi_thres_wm,grp_thres_wm,grp_GM_mask_name,indi_thres_gm,grp_thres_gm,over_write,d_flag,d,steps_,tot_steps)
```
Defined at source line `1`.

### Description
WHIFUN_CREATE_GROUP_MASK Creates group-level White Matter (WM) and Gray Matter (GM) masks. [GROUP_MASK_WM_PATH, GROUP_MASK_GM_PATH, D] = WHIFUN_CREATE_GROUP_MASK(OUT_ANALYSIS_PATH, SUBJ_LIST, GRP_WM_MASK_NAME, INDI_THRES_WM, GRP_THRES_WM, GRP_GM_MASK_NAME, INDI_THRES_GM, GRP_THRES_GM, OVER_WRITE, D_FLAG, D, STEPS_, TOT_STEPS) This function creates group-level WM and GM masks based on individual segmentation maps (e.g., from SPM/CAT) and functional data coverage. Input Arguments: OUT_ANALYSIS_PATH - Main output directory where 'Group_Masks' folder will be created. SUBJ_LIST - Structure array containing subject information, including paths to individual WM ('WM_MNI'), GM ('GM_MNI') segmentatio

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `out_analysis_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `grp_WM_mask_name` — numeric image/header data, commonly X x Y x Z or X x Y x Z x T
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `indi_thres_wm` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `grp_thres_wm` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `grp_GM_mask_name` — numeric image/header data, commonly X x Y x Z or X x Y x Z x T
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `indi_thres_gm` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `grp_thres_gm` — numeric scalar or numeric vector
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
#### `group_mask_WM_path` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

#### `group_mask_GM_path` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

#### `d` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `niftisave`, `reslice_data`, `whifun_create_file`
- **External Dependencies:** MATLAB NIfTI I/O, ANTs command-line suite, BrainNet Viewer
- **Called By:** `main.mlapp:1223/CreateGroupMasksButtonPushed`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `niftisave`, `reslice_data`, `whifun_create_file`
- Related callers: `main.mlapp:1223/CreateGroupMasksButtonPushed`

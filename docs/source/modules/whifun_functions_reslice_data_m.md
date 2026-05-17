# Module Name: `whifun_functions/reslice_data.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment.
- **Key Features:**
  - Handle .nii.gz. Referenced from y_Read.m. YAN Chao-Gan, 151117
  - Internal calls detected: `y_Read`, `y_Write`
  - External dependencies detected: SPM12

## `reslice_data()`

### Syntax
```matlab
function [OutVolume] = reslice_data(InputFile,TargetSpace,hld,wr,OutputFile,nn)
```
Defined at source line `1`.

### Description
Handle .nii.gz. Referenced from y_Read.m. YAN Chao-Gan, 151117

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `InputFile` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `TargetSpace` — numeric time-series matrix, commonly T x R, V x T, or T x R x S
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `hld` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `wr` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `OutputFile` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `nn` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `OutVolume` — numeric image/header data, commonly X x Y x Z or X x Y x Z x T
Output produced by the MATLAB implementation.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `y_Read`, `y_Write`
- **External Dependencies:** SPM12
- **Called By:** `whifun_functions/whifun_create_avg_voxel_level_fc.m:1/whifun_create_avg_voxel_level_fc`, `whifun_functions/whifun_create_avg_voxel_level_fc_GM_with_WM.m:1/whifun_create_avg_voxel_level_fc_GM_with_WM`, `whifun_functions/whifun_create_avg_voxel_level_fc_GM_with_noise.m:1/whifun_create_avg_voxel_level_fc_GM_with_noise`, `whifun_functions/whifun_create_avg_voxel_level_fc_WM_with_GM.m:1/whifun_create_avg_voxel_level_fc_WM_with_GM`, `whifun_functions/whifun_create_avg_voxel_level_fc_multisession.m:1/whifun_create_avg_voxel_level_fc_multisession`, `whifun_functions/whifun_create_avg_voxel_level_fc_noise_with_GM.m:1/whifun_create_avg_voxel_level_fc_noise_with_GM`, `whifun_functions/whifun_create_group_mask.m:1/whifun_create_group_mask`, `whifun_functions/whifun_create_rest_mask.m:1/whifun_create_rest_mask`, `whifun_functions/whifun_get_ts_from_mask.m:1/whifun_get_ts_from_mask`, `whifun_functions/whifun_normalise_preproc.m:1/whifun_normalise_preproc`, `whifun_functions/whifun_smooth_WM_GM_separately_fast.m:1/whifun_smooth_WM_GM_separately_fast`, `whifun_functions/whifun_smooth_WM_GM_separately_fast_MNI_sub_sep.m:1/whifun_smooth_WM_GM_separately_fast_MNI_sub_sep`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `y_Read`, `y_Write`
- Related callers: `whifun_functions/whifun_create_avg_voxel_level_fc.m:1/whifun_create_avg_voxel_level_fc`, `whifun_functions/whifun_create_avg_voxel_level_fc_GM_with_WM.m:1/whifun_create_avg_voxel_level_fc_GM_with_WM`, `whifun_functions/whifun_create_avg_voxel_level_fc_GM_with_noise.m:1/whifun_create_avg_voxel_level_fc_GM_with_noise`, `whifun_functions/whifun_create_avg_voxel_level_fc_WM_with_GM.m:1/whifun_create_avg_voxel_level_fc_WM_with_GM`, `whifun_functions/whifun_create_avg_voxel_level_fc_multisession.m:1/whifun_create_avg_voxel_level_fc_multisession`, `whifun_functions/whifun_create_avg_voxel_level_fc_noise_with_GM.m:1/whifun_create_avg_voxel_level_fc_noise_with_GM`, `whifun_functions/whifun_create_group_mask.m:1/whifun_create_group_mask`, `whifun_functions/whifun_create_rest_mask.m:1/whifun_create_rest_mask`, `whifun_functions/whifun_get_ts_from_mask.m:1/whifun_get_ts_from_mask`, `whifun_functions/whifun_normalise_preproc.m:1/whifun_normalise_preproc`, `whifun_functions/whifun_smooth_WM_GM_separately_fast.m:1/whifun_smooth_WM_GM_separately_fast`, `whifun_functions/whifun_smooth_WM_GM_separately_fast_MNI_sub_sep.m:1/whifun_smooth_WM_GM_separately_fast_MNI_sub_sep`

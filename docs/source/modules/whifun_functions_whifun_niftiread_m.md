# Module Name: `whifun_functions/whifun_niftiread.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_NIFTIREAD Reads a NIfTI file and applies scaling factors. [volume, info] = WHIFUN_NIFTIREAD(image_path) reads a NIfTI file, correctly applying the stored scaling and offset values from the file's header. This is a crucial step for ensuring that the voxel intensity values are interpreted correctly, as many NIfTI files store data as integers to save space and require a scaling factor to be applied for the correct floating-point representation. The function first reads the volume data and the header information using MATLAB's built-in `niftiread` and `niftiinfo` functions. It then applies
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: MATLAB NIfTI I/O

## `whifun_niftiread()`

### Syntax
```matlab
function [volume,info] = whifun_niftiread(image_path)
```
Defined at source line `1`.

### Description
WHIFUN_NIFTIREAD Reads a NIfTI file and applies scaling factors. [volume, info] = WHIFUN_NIFTIREAD(image_path) reads a NIfTI file, correctly applying the stored scaling and offset values from the file's header. This is a crucial step for ensuring that the voxel intensity values are interpreted correctly, as many NIfTI files store data as integers to save space and require a scaling factor to be applied for the correct floating-point representation. The function first reads the volume data and the header information using MATLAB's built-in `niftiread` and `niftiinfo` functions. It then applies the formula: `y = AdditiveOffset + x * MultiplicativeScaling`, where `x` is the raw data and `y` is

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `image_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `volume` — numeric image/header data, commonly X x Y x Z or X x Y x Z x T
Output produced by the MATLAB implementation.

#### `info` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** MATLAB NIfTI I/O
- **Called By:** `main.mlapp:1254/WMGroupMaskButtonPushed`, `main.mlapp:1382/GMGroupMaskButtonPushed`, `whifun_functions/whifun_change_datatype.m:1/whifun_change_datatype`, `whifun_functions/whifun_convert_3d_to_4d_atlas.m:1/whifun_convert_3d_to_4d_atlas`, `whifun_functions/whifun_create_avg_ts.m:1/whifun_create_avg_ts`, `whifun_functions/whifun_create_avg_voxel_level_fc.m:1/whifun_create_avg_voxel_level_fc`, `whifun_functions/whifun_create_avg_voxel_level_fc_multisession.m:1/whifun_create_avg_voxel_level_fc_multisession`, `whifun_functions/whifun_create_brainnet_images.m:1/whifun_create_brainnet_images`, `whifun_functions/whifun_create_fn_from_parrcorr_and_ttest.m:1/whifun_create_fn_from_parrcorr_and_ttest`, `whifun_functions/whifun_create_focus_region_mask_idx.m:1/whifun_create_focus_region_mask_idx`, `whifun_functions/whifun_fsl_fast_seg.m:1/whifun_fsl_fast_seg`, `whifun_functions/whifun_get_ts_from_mask.m:1/whifun_get_ts_from_mask`, `whifun_functions/whifun_qc_nuisance_regression_global_ts.m:1/whifun_qc_nuisance_regression_global_ts`, `whifun_functions/whifun_regress.m:1/whifun_regress`, `whifun_functions/whifun_regress_any.m:1/whifun_regress_any`, `whifun_functions/whifun_seed_corr.m:1/whifun_seed_corr`, `whifun_functions/whifun_seperate_left_right.m:1/whifun_seperate_left_right`, `whifun_functions/whifun_smooth_WM_GM_separately_fast.m:1/whifun_smooth_WM_GM_separately_fast`, `whifun_functions/whifun_smooth_WM_GM_separately_fast_MNI_sub_sep.m:1/whifun_smooth_WM_GM_separately_fast_MNI_sub_sep`, `whifun_functions/whifun_ts_check.m:1/whifun_ts_check`, `whifun_functions/whifun_ts_extract.m:1/whifun_ts_extract`, `whifun_functions/whifun_ts_extract.m:159/extract_ts`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `main.mlapp:1254/WMGroupMaskButtonPushed`, `main.mlapp:1382/GMGroupMaskButtonPushed`, `whifun_functions/whifun_change_datatype.m:1/whifun_change_datatype`, `whifun_functions/whifun_convert_3d_to_4d_atlas.m:1/whifun_convert_3d_to_4d_atlas`, `whifun_functions/whifun_create_avg_ts.m:1/whifun_create_avg_ts`, `whifun_functions/whifun_create_avg_voxel_level_fc.m:1/whifun_create_avg_voxel_level_fc`, `whifun_functions/whifun_create_avg_voxel_level_fc_multisession.m:1/whifun_create_avg_voxel_level_fc_multisession`, `whifun_functions/whifun_create_brainnet_images.m:1/whifun_create_brainnet_images`, `whifun_functions/whifun_create_fn_from_parrcorr_and_ttest.m:1/whifun_create_fn_from_parrcorr_and_ttest`, `whifun_functions/whifun_create_focus_region_mask_idx.m:1/whifun_create_focus_region_mask_idx`, `whifun_functions/whifun_fsl_fast_seg.m:1/whifun_fsl_fast_seg`, `whifun_functions/whifun_get_ts_from_mask.m:1/whifun_get_ts_from_mask`, `whifun_functions/whifun_qc_nuisance_regression_global_ts.m:1/whifun_qc_nuisance_regression_global_ts`, `whifun_functions/whifun_regress.m:1/whifun_regress`, `whifun_functions/whifun_regress_any.m:1/whifun_regress_any`, `whifun_functions/whifun_seed_corr.m:1/whifun_seed_corr`, `whifun_functions/whifun_seperate_left_right.m:1/whifun_seperate_left_right`, `whifun_functions/whifun_smooth_WM_GM_separately_fast.m:1/whifun_smooth_WM_GM_separately_fast`, `whifun_functions/whifun_smooth_WM_GM_separately_fast_MNI_sub_sep.m:1/whifun_smooth_WM_GM_separately_fast_MNI_sub_sep`, `whifun_functions/whifun_ts_check.m:1/whifun_ts_check`, `whifun_functions/whifun_ts_extract.m:1/whifun_ts_extract`, `whifun_functions/whifun_ts_extract.m:159/extract_ts`

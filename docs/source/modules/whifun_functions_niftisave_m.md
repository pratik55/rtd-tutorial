# Module Name: `whifun_functions/niftisave.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - NIFTISAVE Saves a MATLAB array as a NIfTI-1 file, updating essential header information from a provided info structure. NIFTISAVE(NIFTIIMAGE, FILENAME, INFO, ADD_OFFSET, MULTI_SCALE) This is a utility wrapper for MATLAB's built-in `niftiwrite` function. It ensures that the NIfTI header information (INFO) is correctly updated to reflect the dimensions, datatype, and name of the image data being saved. Input Arguments: NIFTIIMAGE - The MATLAB array (2D, 3D, or 4D) containing the image data to be saved as a NIfTI file. FILENAME - The desired full path and filename (with extension, e.g., '.nii') f
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: MATLAB NIfTI I/O

## Function: `niftisave()`
- **Signature & Definition:** `function niftisave(niftiimage,filename,info,add_offset,multi_scale)` (line 1)
- **Scientific Theory & Formulas:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** NIFTISAVE Saves a MATLAB array as a NIfTI-1 file, updating essential header information from a provided info structure. NIFTISAVE(NIFTIIMAGE, FILENAME, INFO, ADD_OFFSET, MULTI_SCALE) This is a utility wrapper for MATLAB's built-in `niftiwrite` function. It ensures that the NIfTI header information (INFO) is correctly updated to reflect the dimensions, datatype, and name of the image data being saved. Input Arguments: NIFTIIMAGE - The MATLAB array (2D, 3D, or 4D) containing the image data to be saved as a NIfTI file. FILENAME - The desired full path and filename (with extension, e.g., '.nii') for the output NIfTI file. INFO - A structure, typically obtained from a previous `niftiread` call, c
- **Arguments:**
  - `niftiimage` (numeric image/header data, commonly X x Y x Z or X x Y x Z x T): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `filename` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `info` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `add_offset` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `multi_scale` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: MATLAB NIfTI I/O
  - Called By: `whifun_functions/dice_iou.m:1/dice_iou`, `whifun_functions/whifun_change_datatype.m:1/whifun_change_datatype`, `whifun_functions/whifun_convert_3d_to_4d_atlas.m:1/whifun_convert_3d_to_4d_atlas`, `whifun_functions/whifun_convert_ROIs_to_atlas.m:1/whifun_convert_ROIs_to_atlas`, `whifun_functions/whifun_create_avg_ts.m:1/whifun_create_avg_ts`, `whifun_functions/whifun_create_fn_from_parrcorr_and_ttest.m:1/whifun_create_fn_from_parrcorr_and_ttest`, `whifun_functions/whifun_create_focus_region_mask_idx.m:1/whifun_create_focus_region_mask_idx`, `whifun_functions/whifun_create_group_mask.m:1/whifun_create_group_mask`, `whifun_functions/whifun_discard_initial_volume_preproc.m:1/whifun_discard_initial_volume_preproc`, `whifun_functions/whifun_erode.m:1/whifun_erode`, `whifun_functions/whifun_filter_preproc.m:1/whifun_filter_preproc`, `whifun_functions/whifun_fsl_fast_seg.m:1/whifun_fsl_fast_seg`, `whifun_functions/whifun_get_FN_kmeans.m:1/whifun_get_FN_kmeans`, `whifun_functions/whifun_regress.m:1/whifun_regress`, `whifun_functions/whifun_regress_any.m:1/whifun_regress_any`, `whifun_functions/whifun_seed_corr.m:1/whifun_seed_corr`, `whifun_functions/whifun_seperate_left_right.m:1/whifun_seperate_left_right`, `whifun_functions/whifun_smooth_WM_GM_separately_fast.m:1/whifun_smooth_WM_GM_separately_fast`, `whifun_functions/whifun_smooth_WM_GM_separately_fast_MNI_sub_sep.m:1/whifun_smooth_WM_GM_separately_fast_MNI_sub_sep`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files.

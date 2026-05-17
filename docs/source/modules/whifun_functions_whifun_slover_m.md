# Module Name: `whifun_functions/whifun_slover.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_SLOVER A wrapper function around the core 'slover' visualization engine, customized for WhiFuN's needs, particularly for image overlays and segmentation QC displays. OBJ = WHIFUN_SLOVER(IMGS, ITYPE, CMAP, SLICES, CNT_RANGE, IMG_VIEW, WT, FG, CBAR_) This function initializes and configures a 'slover' object to display multiple NIfTI images with custom colormaps, slices, and views, and then calls a drawing function (whifun_paint) to render the output. Input Arguments: IMGS - Cell array of full paths to NIfTI files to be displayed. ITYPE - Cell array of strings defining the image type for 
  - Internal calls detected: `whifun_paint`
  - External dependencies detected: SPM12, SLover/MarsBaR-style visualization helpers

## Function: `whifun_slover()`
- **Signature & Definition:** `function obj = whifun_slover(imgs,itype,cmap,slices,cnt_range,img_view,wt,fg,cbar_)` (line 1)
- **Scientific Theory & Formulas:** Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_SLOVER A wrapper function around the core 'slover' visualization engine, customized for WhiFuN's needs, particularly for image overlays and segmentation QC displays. OBJ = WHIFUN_SLOVER(IMGS, ITYPE, CMAP, SLICES, CNT_RANGE, IMG_VIEW, WT, FG, CBAR_) This function initializes and configures a 'slover' object to display multiple NIfTI images with custom colormaps, slices, and views, and then calls a drawing function (whifun_paint) to render the output. Input Arguments: IMGS - Cell array of full paths to NIfTI files to be displayed. ITYPE - Cell array of strings defining the image type for each image (e.g., 'Structural', 'Blobs', 'Truecolour', 'Contours', and related items.). CMAP - Cell array of color
- **Arguments:**
  - `imgs` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `itype` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `cmap` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `slices` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `cnt_range` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `img_view` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `wt` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `fg` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `cbar_` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `obj` (MATLAB App/UI object or callback handle): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `whifun_paint`
  - External: SPM12, SLover/MarsBaR-style visualization helpers
  - Called By: `whifun_functions/whifun_coreg_qc.m:1/whifun_coreg_qc`, `whifun_functions/whifun_ortho_slover_single_image_save.m:1/whifun_ortho_slover_single_image_save`, `whifun_functions/whifun_qc_coreg_slover.m:1/whifun_qc_coreg_slover`, `whifun_functions/whifun_qc_segment.m:1/whifun_qc_segment`, `whifun_functions/whifun_seed_corr_qc_plot.m:1/whifun_seed_corr_qc_plot`, `whifun_functions/whifun_ts_mask_qc.m:1/whifun_ts_mask_qc`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections.

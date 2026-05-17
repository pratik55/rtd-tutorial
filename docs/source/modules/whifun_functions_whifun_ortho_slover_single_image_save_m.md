# Module Name: `whifun_functions/whifun_ortho_slover_single_image_save.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_ORTHO_SLOVER_SINGLE_IMAGE_SAVE Generates and saves an orthogonal view and a 'Slover' visualization of a single NIfTI image, primarily using SPM routines. WHIFUN_ORTHO_SLOVER_SINGLE_IMAGE_SAVE(IMAGE_PATH, OUT_IMAGE_ORTHO_PATH, OUT_IMAGE_SLOVER_PATH, SLICES, CONTOUR_RANGE, VIEW, CAPTION) This function is a utility that takes a NIfTI image, displays it in two different visualization formats (SPM's orthogonal view and a custom Slover-like slice view), and saves the resulting figures to disk. Input Arguments: IMAGE_PATH - Full path to the input NIfTI image file. If 4D, the first volume (',1'
  - Internal calls detected: `spm_check_registration_evalc`, `whifun_slover`
  - External dependencies detected: MATLAB NIfTI I/O, SPM12, SLover/MarsBaR-style visualization helpers

## Function: `whifun_ortho_slover_single_image_save()`
- **Signature & Definition:** `function whifun_ortho_slover_single_image_save(image_path,out_image_ortho_path,out_image_slover_path,slover_slices,slover_contour_range,slover_view,caption_)` (line 1)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_ORTHO_SLOVER_SINGLE_IMAGE_SAVE Generates and saves an orthogonal view and a 'Slover' visualization of a single NIfTI image, primarily using SPM routines. WHIFUN_ORTHO_SLOVER_SINGLE_IMAGE_SAVE(IMAGE_PATH, OUT_IMAGE_ORTHO_PATH, OUT_IMAGE_SLOVER_PATH, SLICES, CONTOUR_RANGE, VIEW, CAPTION) This function is a utility that takes a NIfTI image, displays it in two different visualization formats (SPM's orthogonal view and a custom Slover-like slice view), and saves the resulting figures to disk. Input Arguments: IMAGE_PATH - Full path to the input NIfTI image file. If 4D, the first volume (',1') is automatically selected. OUT_IMAGE_ORTHO_PATH - Full path to save the orthogonal (SPM) view grap
- **Arguments:**
  - `image_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `out_image_ortho_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `out_image_slover_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `slover_slices` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `slover_contour_range` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `slover_view` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `caption_` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: `spm_check_registration_evalc`, `whifun_slover`
  - External: MATLAB NIfTI I/O, SPM12, SLover/MarsBaR-style visualization helpers
  - Called By: `whifun_functions/whifun_qc_smooth.m:1/whifun_qc_smooth`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections.

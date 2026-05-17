# Module Name: `whifun_functions/whifun_create_all_fn_image_montage.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CREATE_ALL_FN_IMAGE_MONTAGE Consolidates network views into a large grid. This function scans a folder for brain network visualizations (PNGs), extracts their network IDs, and tiles them into a large canvas. Each row represents a specific Functional Network (FN), and each column represents a specific anatomical view (Left, Dorsal, Posterior). INPUTS: inputFolder - String. Directory containing the individual network PNGs. outputPrefix - String. Filename prefix for the final montage (e.g., 'Group_ICA'). tissueTypes - Cell Array. e.g., {'WM', 'GM'} to process White and Grey matter. FILE NA
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_create_all_fn_image_montage()`
- **Signature & Definition:** `function whifun_create_all_fn_image_montage(inputFolder, outputPrefix, tissueTypes)` (line 1)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_CREATE_ALL_FN_IMAGE_MONTAGE Consolidates network views into a large grid. This function scans a folder for brain network visualizations (PNGs), extracts their network IDs, and tiles them into a large canvas. Each row represents a specific Functional Network (FN), and each column represents a specific anatomical view (Left, Dorsal, Posterior). INPUTS: inputFolder - String. Directory containing the individual network PNGs. outputPrefix - String. Filename prefix for the final montage (e.g., 'Group_ICA'). tissueTypes - Cell Array. e.g., {'WM', 'GM'} to process White and Grey matter. FILE NAMING CONVENTION EXPECTED: [Tissue]_FN_K[TotalNets]_[NetID]_[View].png Example: GM_FN_K17_5_left.png 
- **Arguments:**
  - `inputFolder` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `outputPrefix` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `tissueTypes` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

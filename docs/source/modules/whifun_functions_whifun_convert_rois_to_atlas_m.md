# Module Name: `whifun_functions/whifun_convert_ROIs_to_atlas.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CONVERT_ROIS_TO_ATLAS Combines multiple binary NIfTI ROI masks into a single labeled NIfTI atlas volume. WHIFUN_CONVERT_ROIS_TO_ATLAS(FOLDER_PATH, PATTERN, OUT_FOLDER) This function reads a collection of NIfTI files, where each file represents a binary Region of Interest (ROI) mask. It then assigns a unique integer label to the voxels belonging to each ROI and saves the result as a single NIfTI atlas file. Input Arguments: FOLDER_PATH - Full path to the directory containing the NIfTI ROI mask files. PATTERN - (Optional, default '') A wildcard pattern (e.g., '*.nii' or 'ROI_*.nii') to ma
  - Internal calls detected: `niftisave`
  - External dependencies detected: MATLAB NIfTI I/O

## Function: `whifun_convert_ROIs_to_atlas()`
- **Signature & Definition:** `function whifun_convert_ROIs_to_atlas(folder_path,pattern,out_path)` (line 1)
- **Scientific Theory & Formulas:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_CONVERT_ROIS_TO_ATLAS Combines multiple binary NIfTI ROI masks into a single labeled NIfTI atlas volume. WHIFUN_CONVERT_ROIS_TO_ATLAS(FOLDER_PATH, PATTERN, OUT_FOLDER) This function reads a collection of NIfTI files, where each file represents a binary Region of Interest (ROI) mask. It then assigns a unique integer label to the voxels belonging to each ROI and saves the result as a single NIfTI atlas file. Input Arguments: FOLDER_PATH - Full path to the directory containing the NIfTI ROI mask files. PATTERN - (Optional, default '') A wildcard pattern (e.g., '*.nii' or 'ROI_*.nii') to match the files to be included as ROIs. If empty, all files in the folder are considered. OUT_FOLDER -
- **Arguments:**
  - `folder_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `pattern` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `out_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: `niftisave`
  - External: MATLAB NIfTI I/O
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files.

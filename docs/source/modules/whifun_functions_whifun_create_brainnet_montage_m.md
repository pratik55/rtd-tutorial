# Module Name: `whifun_functions/whifun_create_brainnet_montage.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - inputFolder : folder containing WM and GM images outputPrefix: prefix for output files (e.g., 'Networks') Will create 'Networks_WM_montage.png' and 'Networks_GM_montage.png' Define tissue types and views tissueTypes = {'WM', 'GM'};
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: BrainNet Viewer

## Function: `whifun_create_brainnet_montage()`
- **Signature & Definition:** `function whifun_create_brainnet_montage(inputFolder, outputPrefix,tissueTypes)` (line 1)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** inputFolder : folder containing WM and GM images outputPrefix: prefix for output files (e.g., 'Networks') Will create 'Networks_WM_montage.png' and 'Networks_GM_montage.png' Define tissue types and views tissueTypes = {'WM', 'GM'};
- **Arguments:**
  - `inputFolder` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `outputPrefix` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `tissueTypes` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: BrainNet Viewer
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

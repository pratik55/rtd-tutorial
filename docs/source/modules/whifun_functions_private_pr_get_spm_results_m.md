# Module Name: `whifun_functions/private/pr_get_spm_results.m`
- **Module Category:** Private visualization/helper dependency.
- **Theoretical Background:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Key Features:**
  - Fetch SPM results and return as point list FORMAT [XYZ, Z, M] = pr_get_spm_results Outputs XYZ - XYZ point list in voxels (empty if not found) Z - values at points in XYZ M - 4x4 voxel -> world transformation matrix __________________________________________________________________________ Matthew Brett $Id: pr_get_spm_results.m 6623 2015-12-03 18:38:08Z guillaume $
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: SPM12

## Function: `pr_get_spm_results()`
- **Signature & Definition:** `function [XYZ, Z, M] = pr_get_spm_results` (line 1)
- **Scientific Theory & Formulas:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Functional Purpose:** Fetch SPM results and return as point list FORMAT [XYZ, Z, M] = pr_get_spm_results Outputs XYZ - XYZ point list in voxels (empty if not found) Z - values at points in XYZ M - 4x4 voxel -> world transformation matrix __________________________________________________________________________ Matthew Brett $Id: pr_get_spm_results.m 6623 2015-12-03 18:38:08Z guillaume $
- **Arguments:**
  - No explicit input arguments.
- **Returns:**
  - `XYZ` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
  - `Z` (numeric scalar or numeric vector): Output produced by the MATLAB implementation.
  - `M` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: SPM12
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

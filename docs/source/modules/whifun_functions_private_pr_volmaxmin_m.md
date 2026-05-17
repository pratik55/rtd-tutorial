# Module Name: `whifun_functions/private/pr_volmaxmin.m`
- **Module Category:** Private visualization/helper dependency.
- **Theoretical Background:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Key Features:**
  - Return max and min value in image volume FORMAT [mx,mn] = pr_volmaxmin(vol) Input vol - image name or vol struct Outputs mx - maximum mn - minimum __________________________________________________________________________ Matthew Brett $Id: pr_volmaxmin.m 6623 2015-12-03 18:38:08Z guillaume $
  - Internal calls detected: `mars_struct`
  - External dependencies detected: SPM12, SLover/MarsBaR-style visualization helpers

## Function: `pr_volmaxmin()`
- **Signature & Definition:** `function [mx,mn] = pr_volmaxmin(vol)` (line 1)
- **Scientific Theory & Formulas:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Functional Purpose:** Return max and min value in image volume FORMAT [mx,mn] = pr_volmaxmin(vol) Input vol - image name or vol struct Outputs mx - maximum mn - minimum __________________________________________________________________________ Matthew Brett $Id: pr_volmaxmin.m 6623 2015-12-03 18:38:08Z guillaume $
- **Arguments:**
  - `vol` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `mx` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
  - `mn` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `mars_struct`
  - External: SPM12, SLover/MarsBaR-style visualization helpers
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

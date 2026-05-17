# Module Name: `whifun_functions/private/pr_basic_ui.m`
- **Module Category:** Private visualization/helper dependency.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - GUI to request parameters for slover routine FORMAT obj = pr_basic_ui(imgs, dispf) GUI requests choices while accepting many defaults imgs - string or cell array of image names to display (defaults to GUI select if no arguments passed) dispf - optional flag: if set, displays overlay (default = 1) __________________________________________________________________________ Matthew Brett $Id: pr_basic_ui.m 6623 2015-12-03 18:38:08Z guillaume $
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: SPM12, SLover/MarsBaR-style visualization helpers

## Function: `pr_basic_ui()`
- **Signature & Definition:** `function obj = pr_basic_ui(imgs, dispf)` (line 1)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** GUI to request parameters for slover routine FORMAT obj = pr_basic_ui(imgs, dispf) GUI requests choices while accepting many defaults imgs - string or cell array of image names to display (defaults to GUI select if no arguments passed) dispf - optional flag: if set, displays overlay (default = 1) __________________________________________________________________________ Matthew Brett $Id: pr_basic_ui.m 6623 2015-12-03 18:38:08Z guillaume $
- **Arguments:**
  - `imgs` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `dispf` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `obj` (MATLAB App/UI object or callback handle): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: SPM12, SLover/MarsBaR-style visualization helpers
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections.

## Function: `sf_return_cmap()`
- **Signature & Definition:** `function cmap = sf_return_cmap(prompt,defmapn)` (line 136)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** GUI to request parameters for slover routine FORMAT obj = pr_basic_ui(imgs, dispf) GUI requests choices while accepting many defaults imgs - string or cell array of image names to display (defaults to GUI select if no arguments passed) dispf - optional flag: if set, displays overlay (default = 1) __________________________________________________________________________ Matthew Brett $Id: pr_basic_ui.m 6623 2015-12-03 18:38:08Z guillaume $
- **Arguments:**
  - `prompt` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `defmapn` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `cmap` (numeric scalar, vector, matrix, or multidimensional array): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: SPM12, SLover/MarsBaR-style visualization helpers
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections.

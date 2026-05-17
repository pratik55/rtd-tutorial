# Module Name: `whifun_functions/private/pr_basic_ui.m`

## Description
- **Module Category:** Private visualization/helper dependency.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - GUI to request parameters for slover routine FORMAT obj = pr_basic_ui(imgs, dispf) GUI requests choices while accepting many defaults imgs - string or cell array of image names to display (defaults to GUI select if no arguments passed) dispf - optional flag: if set, displays overlay (default = 1) __________________________________________________________________________ Matthew Brett $Id: pr_basic_ui.m 6623 2015-12-03 18:38:08Z guillaume $
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: SPM12, SLover/MarsBaR-style visualization helpers

## `pr_basic_ui()`

### Syntax
```matlab
function obj = pr_basic_ui(imgs, dispf)
```
Defined at source line `1`.

### Description
GUI to request parameters for slover routine FORMAT obj = pr_basic_ui(imgs, dispf) GUI requests choices while accepting many defaults imgs - string or cell array of image names to display (defaults to GUI select if no arguments passed) dispf - optional flag: if set, displays overlay (default = 1) __________________________________________________________________________ Matthew Brett $Id: pr_basic_ui.m 6623 2015-12-03 18:38:08Z guillaume $

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `imgs` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `dispf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `obj` — MATLAB App/UI object or callback handle
Output produced by the MATLAB implementation.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** SPM12, SLover/MarsBaR-style visualization helpers
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `sf_return_cmap()`

### Syntax
```matlab
function cmap = sf_return_cmap(prompt,defmapn)
```
Defined at source line `136`.

### Description
GUI to request parameters for slover routine FORMAT obj = pr_basic_ui(imgs, dispf) GUI requests choices while accepting many defaults imgs - string or cell array of image names to display (defaults to GUI select if no arguments passed) dispf - optional flag: if set, displays overlay (default = 1) __________________________________________________________________________ Matthew Brett $Id: pr_basic_ui.m 6623 2015-12-03 18:38:08Z guillaume $

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `prompt` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `defmapn` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `cmap` — numeric scalar, vector, matrix, or multidimensional array
Output produced by the MATLAB implementation.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** SPM12, SLover/MarsBaR-style visualization helpers
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

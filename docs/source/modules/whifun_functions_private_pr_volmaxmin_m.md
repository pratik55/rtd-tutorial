# Module Name: `whifun_functions/private/pr_volmaxmin.m`

## Description
- **Module Category:** Private visualization/helper dependency.
- **Theoretical Background:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Key Features:**
  - Return max and min value in image volume FORMAT [mx,mn] = pr_volmaxmin(vol) Input vol - image name or vol struct Outputs mx - maximum mn - minimum __________________________________________________________________________ Matthew Brett $Id: pr_volmaxmin.m 6623 2015-12-03 18:38:08Z guillaume $
  - Internal calls detected: `mars_struct`
  - External dependencies detected: SPM12, SLover/MarsBaR-style visualization helpers

## `pr_volmaxmin()`

### Syntax
```matlab
function [mx,mn] = pr_volmaxmin(vol)
```
Defined at source line `1`.

### Description
Return max and min value in image volume FORMAT [mx,mn] = pr_volmaxmin(vol) Input vol - image name or vol struct Outputs mx - maximum mn - minimum __________________________________________________________________________ Matthew Brett $Id: pr_volmaxmin.m 6623 2015-12-03 18:38:08Z guillaume $

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `vol` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `mx` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `mn` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Tips
Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Extended Capabilities
- **Internal Calls:** `mars_struct`
- **External Dependencies:** SPM12, SLover/MarsBaR-style visualization helpers
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `mars_struct`

# Module Name: `whifun_functions/private/pr_get_spm_results.m`

## Description
- **Module Category:** Private visualization/helper dependency.
- **Theoretical Background:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Key Features:**
  - Fetch SPM results and return as point list FORMAT [XYZ, Z, M] = pr_get_spm_results Outputs XYZ - XYZ point list in voxels (empty if not found) Z - values at points in XYZ M - 4x4 voxel -> world transformation matrix __________________________________________________________________________ Matthew Brett $Id: pr_get_spm_results.m 6623 2015-12-03 18:38:08Z guillaume $
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: SPM12

## `pr_get_spm_results()`

### Syntax
```matlab
function [XYZ, Z, M] = pr_get_spm_results
```
Defined at source line `1`.

### Description
Fetch SPM results and return as point list FORMAT [XYZ, Z, M] = pr_get_spm_results Outputs XYZ - XYZ point list in voxels (empty if not found) Z - values at points in XYZ M - 4x4 voxel -> world transformation matrix __________________________________________________________________________ Matthew Brett $Id: pr_get_spm_results.m 6623 2015-12-03 18:38:08Z guillaume $

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `XYZ` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `Z` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

#### `M` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Tips
Defines defaults or branches for optional arguments or missing files. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** SPM12
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

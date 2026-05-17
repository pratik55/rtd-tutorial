# Module Name: `whifun_functions/private/pr_matrix2vol.m`

## Description
- **Module Category:** Private visualization/helper dependency.
- **Theoretical Background:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Key Features:**
  - Return (pseudo) vol struct for 3d matrix FORMAT vol = pr_matrix2vol(mat3d,mat) Inputs mat3d - 3D matrix mat - optional 4x4 voxel -> world transformation Outputs vol - kind of SPM vol struct with matrix data added __________________________________________________________________________ Matthew Brett $Id: pr_matrix2vol.m 6623 2015-12-03 18:38:08Z guillaume $
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: SPM12

## `pr_matrix2vol()`

### Syntax
```matlab
function vol = pr_matrix2vol(mat3d, mat)
```
Defined at source line `1`.

### Description
Return (pseudo) vol struct for 3d matrix FORMAT vol = pr_matrix2vol(mat3d,mat) Inputs mat3d - 3D matrix mat - optional 4x4 voxel -> world transformation Outputs vol - kind of SPM vol struct with matrix data added __________________________________________________________________________ Matthew Brett $Id: pr_matrix2vol.m 6623 2015-12-03 18:38:08Z guillaume $

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `mat3d` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `mat` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `vol` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Tips
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

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

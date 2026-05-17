# Module Name: `whifun_functions/private/pr_blobs2vol.m`

## Description
- **Module Category:** Private visualization/helper dependency.
- **Theoretical Background:** Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms.
- **Key Features:**
  - Take XYZ matrix and values and return SPM matrix vol struct FORMAT vol = pr_blobs2vol(xyz,vals,mat) Inputs xyz - 3xN X Y Z coordinate matrix (in voxels) vals - 1xN values, one per coordinate mat - 4x4 voxel->world space transformation Outputs vol - vol struct, with matrix data 'imgdata' field __________________________________________________________________________ Matthew Brett $Id: pr_blobs2vol.m 6623 2015-12-03 18:38:08Z guillaume $
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `pr_blobs2vol()`

### Syntax
```matlab
function vol = pr_blobs2vol(xyz,vals,mat)
```
Defined at source line `1`.

### Description
Take XYZ matrix and values and return SPM matrix vol struct FORMAT vol = pr_blobs2vol(xyz,vals,mat) Inputs xyz - 3xN X Y Z coordinate matrix (in voxels) vals - 1xN values, one per coordinate mat - 4x4 voxel->world space transformation Outputs vol - vol struct, with matrix data 'imgdata' field __________________________________________________________________________ Matthew Brett $Id: pr_blobs2vol.m 6623 2015-12-03 18:38:08Z guillaume $

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `xyz` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `vals` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `mat` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `vol` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

# Module Name: `whifun_functions/private/pr_blobs2vol.m`
- **Module Category:** Private visualization/helper dependency.
- **Theoretical Background:** Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms.
- **Key Features:**
  - Take XYZ matrix and values and return SPM matrix vol struct FORMAT vol = pr_blobs2vol(xyz,vals,mat) Inputs xyz - 3xN X Y Z coordinate matrix (in voxels) vals - 1xN values, one per coordinate mat - 4x4 voxel->world space transformation Outputs vol - vol struct, with matrix data 'imgdata' field __________________________________________________________________________ Matthew Brett $Id: pr_blobs2vol.m 6623 2015-12-03 18:38:08Z guillaume $
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `pr_blobs2vol()`
- **Signature & Definition:** `function vol = pr_blobs2vol(xyz,vals,mat)` (line 1)
- **Scientific Theory & Formulas:** Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms.
- **Functional Purpose:** Take XYZ matrix and values and return SPM matrix vol struct FORMAT vol = pr_blobs2vol(xyz,vals,mat) Inputs xyz - 3xN X Y Z coordinate matrix (in voxels) vals - 1xN values, one per coordinate mat - 4x4 voxel->world space transformation Outputs vol - vol struct, with matrix data 'imgdata' field __________________________________________________________________________ Matthew Brett $Id: pr_blobs2vol.m 6623 2015-12-03 18:38:08Z guillaume $
- **Arguments:**
  - `xyz` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `vals` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `mat` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `vol` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections.

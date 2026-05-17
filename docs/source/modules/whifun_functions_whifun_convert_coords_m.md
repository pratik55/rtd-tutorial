# Module Name: `whifun_functions/whifun_convert_coords.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms.
- **Key Features:**
  - WHIFUN_CONVERT_COORDS Converts coordinates between MNI and voxel space. coord_out = WHIFUN_CONVERT_COORDS(M, coord_in, mode, mat_py) converts a set of 3D coordinates from one coordinate system to another using a 4x4 affine transformation matrix. This function is a fundamental utility for neuroimaging analysis, as it allows for precise mapping of locations between the standard MNI space and a subject voxel space. It can handle both `mni2vox` and `vox2mni` conversions. The function also includes a parameter to handle the difference between 0-based indexing (Python) and 1-based indexing (MATLAB),
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_convert_coords()`
- **Signature & Definition:** `function coord_out = whifun_convert_coords(M, coord_in, mode,mat_py)` (line 1)
- **Scientific Theory & Formulas:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms.
- **Functional Purpose:** WHIFUN_CONVERT_COORDS Converts coordinates between MNI and voxel space. coord_out = WHIFUN_CONVERT_COORDS(M, coord_in, mode, mat_py) converts a set of 3D coordinates from one coordinate system to another using a 4x4 affine transformation matrix. This function is a fundamental utility for neuroimaging analysis, as it allows for precise mapping of locations between the standard MNI space and a subject voxel space. It can handle both `mni2vox` and `vox2mni` conversions. The function also includes a parameter to handle the difference between 0-based indexing (Python) and 1-based indexing (MATLAB), ensuring correct conversion. Input Arguments: M - A 4x4 affine transformation matrix (e.g., from a 
- **Arguments:**
  - `M` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `coord_in` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `mode` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `mat_py` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `coord_out` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: `whifun_functions/whifun_instacorr.m:1/whifun_seed_corr`, `whifun_functions/whifun_seed_corr.m:1/whifun_seed_corr`, `whifun_functions/whifun_view.m:1/whifun_view`, `whifun_functions/whifun_view.m:172/editBoxCallback`, `whifun_functions/whifun_view.m:212/updateViews`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

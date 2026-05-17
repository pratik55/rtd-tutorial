# Module Name: `whifun_functions/whifun_seperate_left_right.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_SEPERATE_LEFT_RIGHT Separates a Functional Network (FN) NIfTI volume into left and right hemispheric components based on the mid-sagittal slice. WHIFUN_SEPERATE_LEFT_RIGHT(FN_FILE_PATH, ONE_IMAGE) This utility function is used to create separate NIfTI files for the left (L) and right (R) halves of a clustered network map (e.g., WM-FN). Input Arguments: FN_FILE_PATH - Full path to the NIfTI file containing the clustered Functional Network. (e.g., 'WM_FN_K10.nii'). ONE_IMAGE - (Optional, default 0) Flag to determine output format: ONE_IMAGE = 0: Saves two separate NIfTI files: '_L' and '_
  - Internal calls detected: `niftisave`, `whifun_niftiread`
  - External dependencies detected: MATLAB NIfTI I/O

## `whifun_seperate_left_right()`

### Syntax
```matlab
function whifun_seperate_left_right(FN_file_path,one_image)
```
Defined at source line `1`.

### Description
WHIFUN_SEPERATE_LEFT_RIGHT Separates a Functional Network (FN) NIfTI volume into left and right hemispheric components based on the mid-sagittal slice. WHIFUN_SEPERATE_LEFT_RIGHT(FN_FILE_PATH, ONE_IMAGE) This utility function is used to create separate NIfTI files for the left (L) and right (R) halves of a clustered network map (e.g., WM-FN). Input Arguments: FN_FILE_PATH - Full path to the NIfTI file containing the clustered Functional Network. (e.g., 'WM_FN_K10.nii'). ONE_IMAGE - (Optional, default 0) Flag to determine output format: ONE_IMAGE = 0: Saves two separate NIfTI files: '_L' and '_R'. ONE_IMAGE = 1: Saves a single NIfTI file '_L_R_seperated' where the right hemisphere's network l

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `FN_file_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `one_image` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files.

### Algorithms
K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `niftisave`, `whifun_niftiread`
- **External Dependencies:** MATLAB NIfTI I/O
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `niftisave`, `whifun_niftiread`

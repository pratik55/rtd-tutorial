# Module Name: `whifun_functions/whifun_extract_ts_from_vox.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms.
- **Key Features:**
  - WHIFUN_EXTRACT_TS_FROM_VOX Extracts time series data from a list of voxels. vox_ts = WHIFUN_EXTRACT_TS_FROM_VOX(func_img, vox_list) extracts the time series data for a specified set of voxels from a 4D functional neuroimaging image volume. The function first reshapes the 4D image data into a 2D matrix where each row represents a voxel and each column represents a time point. It then uses a list of voxel coordinates to extract the corresponding time series. This is an efficient way to get the data for a region of interest (ROI) without having to loop through each voxel. Input Arguments: func_im
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_extract_ts_from_vox()`

### Syntax
```matlab
function vox_ts = whifun_extract_ts_from_vox(func_img,vox_list)
```
Defined at source line `1`.

### Description
WHIFUN_EXTRACT_TS_FROM_VOX Extracts time series data from a list of voxels. vox_ts = WHIFUN_EXTRACT_TS_FROM_VOX(func_img, vox_list) extracts the time series data for a specified set of voxels from a 4D functional neuroimaging image volume. The function first reshapes the 4D image data into a 2D matrix where each row represents a voxel and each column represents a time point. It then uses a list of voxel coordinates to extract the corresponding time series. This is an efficient way to get the data for a region of interest (ROI) without having to loop through each voxel. Input Arguments: func_img - A 4D matrix of functional image data `[nx ny nz nt]`. vox_list - An Nx3 array of voxel coordinat

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `func_img` — numeric image/header data, commonly X x Y x Z or X x Y x Z x T
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `vox_list` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `vox_ts` — numeric time-series matrix, commonly T x R, V x T, or T x R x S
Output produced by the MATLAB implementation.

### More About
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** `whifun_functions/whifun_instacorr.m:1/whifun_seed_corr`, `whifun_functions/whifun_seed_corr.m:1/whifun_seed_corr`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `whifun_functions/whifun_instacorr.m:1/whifun_seed_corr`, `whifun_functions/whifun_seed_corr.m:1/whifun_seed_corr`

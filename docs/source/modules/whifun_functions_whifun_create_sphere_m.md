# Module Name: `whifun_functions/whifun_create_sphere.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms.
- **Key Features:**
  - WHIFUN_CREATE_SPHERE Generates a list of voxel coordinates within a sphere. vox_list = WHIFUN_CREATE_SPHERE(center_vox, radius_mm, vox_dim, vol_size) creates a list of 1-based voxel coordinates that fall inside a sphere of a given radius. This function is a core utility for defining spherical regions of interest (ROIs) in neuroimaging analysis. The function first calculates a cubic grid of candidate voxels around the center point. It then filters this grid, keeping only the voxels whose Euclidean distance from the center (in millimeters) is less than or equal to the specified radius. Finally,
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_create_sphere()`

### Syntax
```matlab
function vox_list = whifun_create_sphere(center_vox, radius_mm, vox_dim, vol_size)
```
Defined at source line `1`.

### Description
WHIFUN_CREATE_SPHERE Generates a list of voxel coordinates within a sphere. vox_list = WHIFUN_CREATE_SPHERE(center_vox, radius_mm, vox_dim, vol_size) creates a list of 1-based voxel coordinates that fall inside a sphere of a given radius. This function is a core utility for defining spherical regions of interest (ROIs) in neuroimaging analysis. The function first calculates a cubic grid of candidate voxels around the center point. It then filters this grid, keeping only the voxels whose Euclidean distance from the center (in millimeters) is less than or equal to the specified radius. Finally, it clips the list of voxels to ensure they are all within the bounds of the image volume. Input Argu

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `center_vox` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `radius_mm` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `vox_dim` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `vol_size` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `vox_list` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

### More About
Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** `whifun_functions/whifun_instacorr.m:1/whifun_seed_corr`, `whifun_functions/whifun_seed_corr.m:1/whifun_seed_corr`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `whifun_functions/whifun_instacorr.m:1/whifun_seed_corr`, `whifun_functions/whifun_seed_corr.m:1/whifun_seed_corr`

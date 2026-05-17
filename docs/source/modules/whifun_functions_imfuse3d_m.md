# Module Name: `whifun_functions/imfuse3d.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - IMFUSE3D Performs slice-wise image fusion for 3D volumes. OUT = IMFUSE3D(A, B) iterates through the third dimension of two volumes, A and B, and fuses each corresponding pair of 2D slices using the IMFUSE function. The resulting color composite is converted back to grayscale by taking the mean across color channels. INPUTS: A - A 3D numeric array (e.g., anatomical reference). B - A 3D numeric array of the same size as A (e.g., overlay). OUTPUTS: out - A 3D numeric array containing the fused intensity values. EXAMPLE: % Fuse a T1 anatomical with a T2 or functional volume fused_vol = imfuse3d(t1
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: Image Processing Toolbox

## `imfuse3d()`

### Syntax
```matlab
function out = imfuse3d(A,B)
```
Defined at source line `1`.

### Description
IMFUSE3D Performs slice-wise image fusion for 3D volumes. OUT = IMFUSE3D(A, B) iterates through the third dimension of two volumes, A and B, and fuses each corresponding pair of 2D slices using the IMFUSE function. The resulting color composite is converted back to grayscale by taking the mean across color channels. INPUTS: A - A 3D numeric array (e.g., anatomical reference). B - A 3D numeric array of the same size as A (e.g., overlay). OUTPUTS: out - A 3D numeric array containing the fused intensity values. EXAMPLE: % Fuse a T1 anatomical with a T2 or functional volume fused_vol = imfuse3d(t1_vol, t2_vol); whifun_figure_montage(fused_vol, 8, 8); NOTES: - This function requires the Image Pro

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `A` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `B` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `out` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** Image Processing Toolbox
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

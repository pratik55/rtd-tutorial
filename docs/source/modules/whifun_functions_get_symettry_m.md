# Module Name: `whifun_functions/get_symettry.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms.
- **Key Features:**
  - GET_SYMETTRY Measures the spatial symmetry of a functional network clustering solution by comparing the clustering patterns in the Left and Right hemispheres. DICE_COEF_LR = GET_SYMETTRY(CURRENT_CLUSTERING_SOLUTION) This function quantifies the degree to which a functional network solution is mirror-symmetric across the mid-sagittal plane. It achieves this by: 1. Separating the clustering volume into Left (L) and Right (R) halves. 2. Flipping the Right half along the Left-Right axis (Dim 1) so it aligns with the Left half. 3. Masking both halves to only include voxels present in both. 4. Conve
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `get_symettry()`

### Syntax
```matlab
function Dice_coef_LR = get_symettry(current_clustering_solution)
```
Defined at source line `1`.

### Description
GET_SYMETTRY Measures the spatial symmetry of a functional network clustering solution by comparing the clustering patterns in the Left and Right hemispheres. DICE_COEF_LR = GET_SYMETTRY(CURRENT_CLUSTERING_SOLUTION) This function quantifies the degree to which a functional network solution is mirror-symmetric across the mid-sagittal plane. It achieves this by: 1. Separating the clustering volume into Left (L) and Right (R) halves. 2. Flipping the Right half along the Left-Right axis (Dim 1) so it aligns with the Left half. 3. Masking both halves to only include voxels present in both. 4. Converting the L and R clustering solutions into Adjacency Matrices (AMs) based on whether pairs of voxel

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `current_clustering_solution` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Dice_coef_LR` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

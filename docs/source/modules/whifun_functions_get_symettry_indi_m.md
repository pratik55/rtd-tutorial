# Module Name: `whifun_functions/get_symettry_indi.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms.
- **Key Features:**
  - GET_SYMETTRY_INDI Measures the spatial symmetry of a functional network clustering solution using the Dice similarity coefficient, leveraging an external `dice_iou` function. DICE_COEF_LR = GET_SYMETTRY_INDI(CURRENT_CLUSTERING_SOLUTION) This function quantifies the degree of mirror-symmetry for a single clustering solution across the mid-sagittal plane. It compares the network labels in the Left hemisphere with the mirrored network labels from the Right hemisphere using the Dice coefficient. Input Arguments: CURRENT_CLUSTERING_SOLUTION - A 3D NIfTI volume (X x Y x Z) where each non-zero voxel 
  - Internal calls detected: `dice_iou`
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `get_symettry_indi()`
- **Signature & Definition:** `function Dice_coef_LR = get_symettry_indi(current_clustering_solution)` (line 1)
- **Scientific Theory & Formulas:** K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms.
- **Functional Purpose:** GET_SYMETTRY_INDI Measures the spatial symmetry of a functional network clustering solution using the Dice similarity coefficient, leveraging an external `dice_iou` function. DICE_COEF_LR = GET_SYMETTRY_INDI(CURRENT_CLUSTERING_SOLUTION) This function quantifies the degree of mirror-symmetry for a single clustering solution across the mid-sagittal plane. It compares the network labels in the Left hemisphere with the mirrored network labels from the Right hemisphere using the Dice coefficient. Input Arguments: CURRENT_CLUSTERING_SOLUTION - A 3D NIfTI volume (X x Y x Z) where each non-zero voxel contains a cluster/network label (K). Output Arguments: DICE_COEF_LR - The Dice similarity coefficie
- **Arguments:**
  - `current_clustering_solution` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `Dice_coef_LR` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `dice_iou`
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

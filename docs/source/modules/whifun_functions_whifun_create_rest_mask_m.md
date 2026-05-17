# Module Name: `whifun_functions/whifun_create_rest_mask.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CREATE_REST_MASK Creates a brain mask in functional space. [REST_MASK1, func_mask_path] = WHIFUN_CREATE_REST_MASK(in_func_path, in_anat_mask_subj_space_path) creates a brain mask for a functional image based on a pre-existing anatomical brain mask. This is a crucial step for subsequent analysis that needs to be restricted to brain tissue. The function uses `reslice_data` (an assumed helper function, as it is not a standard MATLAB function) to resample the anatomical mask into the functional image's space. Reslicing ensures that the mask has the same dimensions and voxel-to-world mapping
  - Internal calls detected: `reslice_data`
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_create_rest_mask()`
- **Signature & Definition:** `function [REST_MASK1,func_mask_path] = whifun_create_rest_mask(in_func_path,in_anat_mask_subj_space_path)` (line 1)
- **Scientific Theory & Formulas:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_CREATE_REST_MASK Creates a brain mask in functional space. [REST_MASK1, func_mask_path] = WHIFUN_CREATE_REST_MASK(in_func_path, in_anat_mask_subj_space_path) creates a brain mask for a functional image based on a pre-existing anatomical brain mask. This is a crucial step for subsequent analysis that needs to be restricted to brain tissue. The function uses `reslice_data` (an assumed helper function, as it is not a standard MATLAB function) to resample the anatomical mask into the functional image's space. Reslicing ensures that the mask has the same dimensions and voxel-to-world mapping as the functional data, allowing for direct application. Input Arguments: in_func_path - The path t
- **Arguments:**
  - `in_func_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `in_anat_mask_subj_space_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `REST_MASK1` (numeric image/header data, commonly X x Y x Z or X x Y x Z x T): Output produced by the MATLAB implementation.
  - `func_mask_path` (character vector or string scalar filesystem path): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `reslice_data`
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: `whifun_functions/whifun_preproc.m:1/whifun_preproc`, `whifun_functions/whifun_preproc_fsl.m:1/whifun_preproc_fsl`, `whifun_functions/whifun_regress.m:1/whifun_regress`, `whifun_functions/whifun_regress_any.m:1/whifun_regress_any`
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

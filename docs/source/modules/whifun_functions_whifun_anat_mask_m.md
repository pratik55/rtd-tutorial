# Module Name: `whifun_functions/whifun_anat_mask.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_WANAT_MASK Creates a brain mask from segmented anatomical images in MNI space using SPM. output = WHIFUN_ANAT_MASK(m_file, now_anat_path, norm) creates a binary brain mask by combining the segmented Gray Matter (GM), White Matter (WM), and Cerebrospinal Fluid (CSF) images. This function configures and runs the `imcalc` module in SPM to perform a simple logical operation. It sums the segmented GM, WM, and CSF images and creates a binary mask where any voxel with a combined probability greater than 0.5 is set to 1 (brain tissue), and all other voxels are set to 0. The function can create 
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: SPM12, Shell/system execution

## Function: `whifun_anat_mask()`
- **Signature & Definition:** `function output = whifun_anat_mask(out_mask_path,anat_path,GM_path,WM_path,CSF_path)` (line 1)
- **Scientific Theory & Formulas:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_WANAT_MASK Creates a brain mask from segmented anatomical images in MNI space using SPM. output = WHIFUN_ANAT_MASK(m_file, now_anat_path, norm) creates a binary brain mask by combining the segmented Gray Matter (GM), White Matter (WM), and Cerebrospinal Fluid (CSF) images. This function configures and runs the `imcalc` module in SPM to perform a simple logical operation. It sums the segmented GM, WM, and CSF images and creates a binary mask where any voxel with a combined probability greater than 0.5 is set to 1 (brain tissue), and all other voxels are set to 0. The function can create the mask in either native or MNI space, based on the `norm` input argument. This is a crucial step f
- **Arguments:**
  - `out_mask_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `anat_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `GM_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `WM_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `CSF_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `output` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: SPM12, Shell/system execution
  - Called By: `whifun_functions/whifun_normalise_preproc.m:1/whifun_normalise_preproc`, `whifun_functions/whifun_skull_strip_and_anat_mask_preproc.m:1/whifun_skull_strip_and_anat_mask_preproc`
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

# Module Name: `whifun_functions/whifun_create_seg_overlaps.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CREATE_SEG_OVERLAPS Visualizes the overlap of Gray Matter (GM), White Matter (WM), and Cerebrospinal Fluid (CSF) segmentation masks onto a reference image using SPM's `spm_orthviews`. WHIFUN_CREATE_SEG_OVERLAPS(GM_PATH, WM_PATH, CSF_PATH, REF, CAPTION_1, CAPTION_2) This function is used for quality control (QC) in neuroimaging pipelines, allowing a visual check of the accuracy of tissue segmentation (e.g., from SPM's 'New Segment' or 'Segment' tools) by overlaying the masks in distinct colors onto a T1-weighted or normalized reference image. Input Arguments: GM_PATH - Full path to the N
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: SPM12, Shell/system execution

## Function: `whifun_create_seg_overlaps()`
- **Signature & Definition:** `function whifun_create_seg_overlaps(GM_path,WM_path,CSF_path,ref,caption_1,caption_2)` (line 1)
- **Scientific Theory & Formulas:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_CREATE_SEG_OVERLAPS Visualizes the overlap of Gray Matter (GM), White Matter (WM), and Cerebrospinal Fluid (CSF) segmentation masks onto a reference image using SPM's `spm_orthviews`. WHIFUN_CREATE_SEG_OVERLAPS(GM_PATH, WM_PATH, CSF_PATH, REF, CAPTION_1, CAPTION_2) This function is used for quality control (QC) in neuroimaging pipelines, allowing a visual check of the accuracy of tissue segmentation (e.g., from SPM's 'New Segment' or 'Segment' tools) by overlaying the masks in distinct colors onto a T1-weighted or normalized reference image. Input Arguments: GM_PATH - Full path to the NIfTI file containing the Gray Matter segmentation mask (e.g., c1T1.nii). WM_PATH - Full path to the 
- **Arguments:**
  - `GM_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `WM_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `CSF_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `ref` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `caption_1` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `caption_2` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: SPM12, Shell/system execution
  - Called By: `whifun_functions/whifun_qc_segment.m:1/whifun_qc_segment`
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

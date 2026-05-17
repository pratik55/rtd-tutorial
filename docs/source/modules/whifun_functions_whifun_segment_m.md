# Module Name: `whifun_functions/whifun_segment.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_SEGMENT Performs SPM-based segmentation and normalization. output = WHIFUN_SEGMENT(now_anat_path, spm_path) runs the SPM segmentation and normalization routine on a subject's anatomical image. This function configures and executes the `spm_jobman` for the `spm.spatial.preproc` module. The batch job is set up to: - **Bias Correct** the anatomical image and save the output. - **Segment** the image into six tissue types (Gray Matter, White Matter, CSF, skull, and related items.) using the default Tissue Probability Map (TPM). - **Save** the native-space and MNI-normalized versions of the GM, WM, and CSF
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: MATLAB NIfTI I/O, SPM12, Shell/system execution

## `whifun_segment()`

### Syntax
```matlab
function output = whifun_segment(now_anat_path,spm_path)
```
Defined at source line `1`.

### Description
WHIFUN_SEGMENT Performs SPM-based segmentation and normalization. output = WHIFUN_SEGMENT(now_anat_path, spm_path) runs the SPM segmentation and normalization routine on a subject's anatomical image. This function configures and executes the `spm_jobman` for the `spm.spatial.preproc` module. The batch job is set up to: - **Bias Correct** the anatomical image and save the output. - **Segment** the image into six tissue types (Gray Matter, White Matter, CSF, skull, and related items.) using the default Tissue Probability Map (TPM). - **Save** the native-space and MNI-normalized versions of the GM, WM, and CSF segments. - **Save** the forward and inverse deformation field maps, which are essential for normal

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `now_anat_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `spm_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `output` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** MATLAB NIfTI I/O, SPM12, Shell/system execution
- **Called By:** `whifun_functions/whifun_segment_preproc.m:1/whifun_segment_preproc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `whifun_functions/whifun_segment_preproc.m:1/whifun_segment_preproc`

# Module Name: `whifun_functions/whifun_normalise.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_NORMALISE Normalizes images to MNI space using SPM. output = WHIFUN_NORMALISE(in_def_path, ..., func_anat) applies a pre-existing deformation field to either a functional or an anatomical image, transforming it from the subject's native space to a standard template space (MNI). setenv The function configures and executes the `spm.spatial.normalise.write` job. The process involves: 1. **Inputting Deformation Field**: It takes the deformation field (generated during the segmentation step) as the key input for the transformation. 2. **Resampling**: Based on the `func_anat` flag, it either
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: SPM12, Shell/system execution

## `whifun_normalise()`

### Syntax
```matlab
function output = whifun_normalise(in_def_path,in_func_path,in_anat_path,nt,vox,Norm_pre,func_anat)
```
Defined at source line `1`.

### Description
WHIFUN_NORMALISE Normalizes images to MNI space using SPM. output = WHIFUN_NORMALISE(in_def_path, ..., func_anat) applies a pre-existing deformation field to either a functional or an anatomical image, transforming it from the subject's native space to a standard template space (MNI). setenv The function configures and executes the `spm.spatial.normalise.write` job. The process involves: 1. **Inputting Deformation Field**: It takes the deformation field (generated during the segmentation step) as the key input for the transformation. 2. **Resampling**: Based on the `func_anat` flag, it either resamples the entire functional time series or the anatomical image. 3. **Output Voxel Size**: The o

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `in_def_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `in_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `in_anat_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `nt` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `vox` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Norm_pre` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `func_anat` — MATLAB value inferred from source usage
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
- **External Dependencies:** SPM12, Shell/system execution
- **Called By:** `whifun_functions/whifun_normalise_preproc.m:1/whifun_normalise_preproc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `whifun_functions/whifun_normalise_preproc.m:1/whifun_normalise_preproc`

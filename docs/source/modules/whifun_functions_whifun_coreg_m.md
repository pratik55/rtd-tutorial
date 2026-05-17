# Module Name: `whifun_functions/whifun_coreg.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_COREG Performs coregistration using SPM. output = WHIFUN_COREG(now_anat_path, now_func_path, mean_func, nt) aligns a subject's functional images to their anatomical image. This is a critical step in fMRI preprocessing to ensure that functional data can be accurately localized to anatomical structures. The function configures and runs the SPM coregistration job. The anatomical image is set as the reference, and a mean functional image is set as the source. All functional volumes are included as "other" images, ensuring that the same transformation is applied to the entire time series. Ke
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: SPM12, Shell/system execution

## `whifun_coreg()`

### Syntax
```matlab
function output = whifun_coreg(now_anat_path,now_func_path,mean_func,nt)
```
Defined at source line `1`.

### Description
WHIFUN_COREG Performs coregistration using SPM. output = WHIFUN_COREG(now_anat_path, now_func_path, mean_func, nt) aligns a subject's functional images to their anatomical image. This is a critical step in fMRI preprocessing to ensure that functional data can be accurately localized to anatomical structures. The function configures and runs the SPM coregistration job. The anatomical image is set as the reference, and a mean functional image is set as the source. All functional volumes are included as "other" images, ensuring that the same transformation is applied to the entire time series. Key parameters are set for the job: - **Cost Function**: Normalized Mutual Information (`'nmi'`) is us

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `now_anat_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `now_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `mean_func` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `nt` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `output` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Normalized mutual information is $NMI=\frac{2I(X;Y)}{H(X)+H(Y)}$, where $I(X;Y)=\sum_{ij}p_{ij}\log_2\frac{p_{ij}}{p_i p_j}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Normalized mutual information is $NMI=\frac{2I(X;Y)}{H(X)+H(Y)}$, where $I(X;Y)=\sum_{ij}p_{ij}\log_2\frac{p_{ij}}{p_i p_j}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** SPM12, Shell/system execution
- **Called By:** `whifun_functions/whifun_coreg_preproc.m:1/whifun_coreg_preproc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `whifun_functions/whifun_coreg_preproc.m:1/whifun_coreg_preproc`

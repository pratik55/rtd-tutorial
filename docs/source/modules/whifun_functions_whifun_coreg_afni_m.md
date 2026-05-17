# Module Name: `whifun_functions/whifun_coreg_afni.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_COREG_AFNI Performs T2*-to-T1 coregistration using AFNI's `align_epi_anat.py` and cleans up intermediate files. OUTPUT = WHIFUN_COREG_AFNI(NOW_ANAT_PATH, NOW_FUNC_PATH) This function executes a coregistration step, aligning the functional EPI image (T2*) to the anatomical image (T1) using the AFNI (Analysis of Functional NeuroImages) tool `align_epi_anat.py`. It is designed to be used within a MATLAB pipeline, capturing command line output and managing temporary files. Input Arguments: NOW_ANAT_PATH - A structure array (e.g., from `dir` or custom function) pointing to the anatomical (T1
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: AFNI command-line suite, Shell/system execution

## `whifun_coreg_afni()`

### Syntax
```matlab
function output = whifun_coreg_afni(now_anat_path,now_func_path)
```
Defined at source line `1`.

### Description
WHIFUN_COREG_AFNI Performs T2*-to-T1 coregistration using AFNI's `align_epi_anat.py` and cleans up intermediate files. OUTPUT = WHIFUN_COREG_AFNI(NOW_ANAT_PATH, NOW_FUNC_PATH) This function executes a coregistration step, aligning the functional EPI image (T2*) to the anatomical image (T1) using the AFNI (Analysis of Functional NeuroImages) tool `align_epi_anat.py`. It is designed to be used within a MATLAB pipeline, capturing command line output and managing temporary files. Input Arguments: NOW_ANAT_PATH - A structure array (e.g., from `dir` or custom function) pointing to the anatomical (T1) NIfTI file. Must contain fields `folder` and `name`. NOW_FUNC_PATH - A structure array (must conta

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `now_anat_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `now_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `output` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Depends on external command availability and shell exit status.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** AFNI command-line suite, Shell/system execution
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

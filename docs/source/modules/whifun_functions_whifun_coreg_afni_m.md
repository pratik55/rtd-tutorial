# Module Name: `whifun_functions/whifun_coreg_afni.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_COREG_AFNI Performs T2*-to-T1 coregistration using AFNI's `align_epi_anat.py` and cleans up intermediate files. OUTPUT = WHIFUN_COREG_AFNI(NOW_ANAT_PATH, NOW_FUNC_PATH) This function executes a coregistration step, aligning the functional EPI image (T2*) to the anatomical image (T1) using the AFNI (Analysis of Functional NeuroImages) tool `align_epi_anat.py`. It is designed to be used within a MATLAB pipeline, capturing command line output and managing temporary files. Input Arguments: NOW_ANAT_PATH - A structure array (e.g., from `dir` or custom function) pointing to the anatomical (T1
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: AFNI command-line suite, Shell/system execution

## Function: `whifun_coreg_afni()`
- **Signature & Definition:** `function output = whifun_coreg_afni(now_anat_path,now_func_path)` (line 1)
- **Scientific Theory & Formulas:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_COREG_AFNI Performs T2*-to-T1 coregistration using AFNI's `align_epi_anat.py` and cleans up intermediate files. OUTPUT = WHIFUN_COREG_AFNI(NOW_ANAT_PATH, NOW_FUNC_PATH) This function executes a coregistration step, aligning the functional EPI image (T2*) to the anatomical image (T1) using the AFNI (Analysis of Functional NeuroImages) tool `align_epi_anat.py`. It is designed to be used within a MATLAB pipeline, capturing command line output and managing temporary files. Input Arguments: NOW_ANAT_PATH - A structure array (e.g., from `dir` or custom function) pointing to the anatomical (T1) NIfTI file. Must contain fields `folder` and `name`. NOW_FUNC_PATH - A structure array (must conta
- **Arguments:**
  - `now_anat_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `now_func_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `output` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: AFNI command-line suite, Shell/system execution
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Depends on external command availability and shell exit status.

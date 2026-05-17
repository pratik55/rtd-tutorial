# Module Name: `whifun_functions/whifun_fsl_fast_seg.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_FSL_FAST_SEG Performs anatomical segmentation with optional skull stripping using FSL. [gm_prob_path, wm_prob_path, csf_prob_path] = WHIFUN_FSL_FAST_SEG(t1_path, out_dir, do_skullstrip) is a MATLAB wrapper function that automates the process of performing anatomical segmentation using FSL's `fast` tool. It also provides an option to run FSL's `bet` for skull stripping prior to segmentation. The function performs the following steps: 1. **Skull Stripping (optional)**: If `do_skullstrip` is true, it uses `bet` to remove non-brain tissue from the T1 image, saving a new file with `_brain` a
  - Internal calls detected: `niftisave`, `whifun_niftiread`
  - External dependencies detected: MATLAB NIfTI I/O, FSL command-line suite, Shell/system execution

## Function: `whifun_fsl_fast_seg()`
- **Signature & Definition:** `function [gm_prob_path, wm_prob_path, csf_prob_path,t1_input_brain] = whifun_fsl_fast_seg(t1_path, out_dir, do_skullstrip)` (line 1)
- **Scientific Theory & Formulas:** Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_FSL_FAST_SEG Performs anatomical segmentation with optional skull stripping using FSL. [gm_prob_path, wm_prob_path, csf_prob_path] = WHIFUN_FSL_FAST_SEG(t1_path, out_dir, do_skullstrip) is a MATLAB wrapper function that automates the process of performing anatomical segmentation using FSL's `fast` tool. It also provides an option to run FSL's `bet` for skull stripping prior to segmentation. The function performs the following steps: 1. **Skull Stripping (optional)**: If `do_skullstrip` is true, it uses `bet` to remove non-brain tissue from the T1 image, saving a new file with `_brain` appended to its name. 2. **Segmentation**: It then runs `fast` on either the original T1 image or the
- **Arguments:**
  - `t1_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `out_dir` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `do_skullstrip` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `gm_prob_path` (character vector or string scalar filesystem path): Output produced by the MATLAB implementation.
  - `wm_prob_path` (character vector or string scalar filesystem path): Output produced by the MATLAB implementation.
  - `csf_prob_path` (character vector or string scalar filesystem path): Output produced by the MATLAB implementation.
  - `t1_input_brain` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `niftisave`, `whifun_niftiread`
  - External: MATLAB NIfTI I/O, FSL command-line suite, Shell/system execution
  - Called By: `whifun_functions/whifun_post_proc_hcp_dev.m:1/whifun_post_proc_hcp_dev`, `whifun_functions/whifun_preproc_fsl.m:1/whifun_preproc_fsl`, `whifun_functions/whifun_using_other_preproc_segment_fsl.m:1/whifun_using_other_preproc_segment_fsl`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands. Depends on external command availability and shell exit status.

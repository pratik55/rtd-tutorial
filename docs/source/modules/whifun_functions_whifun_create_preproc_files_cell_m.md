# Module Name: `whifun_functions/whifun_create_preproc_files_cell.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - assembleInputs Create a 10x2 cell with variable names and values. finalData = assembleInputs(final_func_MNI, GM_MNI, WM_MNI, CSF_MNI) assembleInputs(..., motion_txt, anat_mask_MNI, func_MNI, anat_MNI, func_mask_MNI, MNI_template) Compulsory inputs (in order): final_func_MNI, GM_MNI, WM_MNI, CSF_MNI Optional inputs (in order). If omitted, they default to empty string: motion_txt, anat_mask_MNI, func_MNI, anat_MNI, func_mask_MNI, MNI_template Output: finalData - 10x2 cell: first column variable names (strings), second column variable values. Validate number of compulsory inputs % ---------------
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_create_preproc_files_cell()`
- **Signature & Definition:** `function finalData = whifun_create_preproc_files_cell(final_func_MNI, GM_MNI, WM_MNI, CSF_MNI, varargin)` (line 1)
- **Scientific Theory & Formulas:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** assembleInputs Create a 10x2 cell with variable names and values. finalData = assembleInputs(final_func_MNI, GM_MNI, WM_MNI, CSF_MNI) assembleInputs(..., motion_txt, anat_mask_MNI, func_MNI, anat_MNI, func_mask_MNI, MNI_template) Compulsory inputs (in order): final_func_MNI, GM_MNI, WM_MNI, CSF_MNI Optional inputs (in order). If omitted, they default to empty string: motion_txt, anat_mask_MNI, func_MNI, anat_MNI, func_mask_MNI, MNI_template Output: finalData - 10x2 cell: first column variable names (strings), second column variable values. Validate number of compulsory inputs % ---------------- Input Parser ----------------
- **Arguments:**
  - `final_func_MNI` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `GM_MNI` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `WM_MNI` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `CSF_MNI` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `finalData` (numeric scalar, vector, matrix, or multidimensional array): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Uses explicit parameter parsing or validation.

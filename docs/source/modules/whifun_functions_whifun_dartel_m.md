# Module Name: `whifun_functions/whifun_dartel.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - % Create Dartel Template output_folder = 'C:\Users\jainp\Box\practice_NY_op_home_laptop'; load(fullfile(output_folder,'parameters.mat')); Subj_list = load_subjects(output_folder,'Subj_list.csv'); Anatomical Dartel Imports - Grey Matter & White Matter & CSF
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: MATLAB table/file I/O, SPM12, Shell/system execution

## Function: `whifun_dartel()`
- **Signature & Definition:** `function output = whifun_dartel(Subj_list)` (line 8)
- **Scientific Theory & Formulas:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment.
- **Functional Purpose:** Anatomical Dartel Imports - Grey Matter & White Matter & CSF
- **Arguments:**
  - `Subj_list` (structure array containing participant metadata and paths): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `output` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: SPM12, Shell/system execution
  - Called By: `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

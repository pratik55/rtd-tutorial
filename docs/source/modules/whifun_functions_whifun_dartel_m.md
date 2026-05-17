# Module Name: `whifun_functions/whifun_dartel.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - % Create Dartel Template output_folder = 'C:\Users\jainp\Box\practice_NY_op_home_laptop'; load(fullfile(output_folder,'parameters.mat')); Subj_list = load_subjects(output_folder,'Subj_list.csv'); Anatomical Dartel Imports - Grey Matter & White Matter & CSF
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: MATLAB table/file I/O, SPM12, Shell/system execution

## `whifun_dartel()`

### Syntax
```matlab
function output = whifun_dartel(Subj_list)
```
Defined at source line `8`.

### Description
Anatomical Dartel Imports - Grey Matter & White Matter & CSF

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `Subj_list` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `output` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** SPM12, Shell/system execution
- **Called By:** `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`

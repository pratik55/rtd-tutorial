# Module Name: `whifun_functions/whifun_reslice_data.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - Reference image (the one you want to match) TargetSpace = 'fmri_img1.nii'; % [47 59 51 200] Source image (the one you want to reslice) InputFile = 'fmri_img2.nii'; % [59 70 60 200] Load both into a char array for spm_reslice
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: SPM12

## `whifun_reslice_data()`

### Syntax
```matlab
function whifun_reslice_data(InputFile,TargetSpace,out_path,interpo)
```
Defined at source line `1`.

### Description
Reference image (the one you want to match) TargetSpace = 'fmri_img1.nii'; % [47 59 51 200] Source image (the one you want to reslice) InputFile = 'fmri_img2.nii'; % [59 70 60 200] Load both into a char array for spm_reslice

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `InputFile` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `TargetSpace` — numeric time-series matrix, commonly T x R, V x T, or T x R x S
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `out_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `interpo` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** SPM12
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

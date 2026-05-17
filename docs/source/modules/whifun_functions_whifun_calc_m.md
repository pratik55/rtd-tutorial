# Module Name: `whifun_functions/whifun_calc.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - whifun_calc(output_path, expression, nifti1, nifti2, ...) Calculates a mathematical expression using multiple NIfTI images. Example: whifun_calc('out.nii', 'i1 + i2 + i3', 'sub1.nii', 'sub2.nii', 'sub3.nii') Inputs: output_path : path to save the output NIfTI file expression : expression to evaluate (e.g., 'i1 + i2 - i3') varargin : list of NIfTI image file paths (all in same grid/space) The variables in the expression must be named i1, i2, i3, ... corresponding to the order of NIfTI inputs.
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: SPM12

## `whifun_calc()`

### Syntax
```matlab
function whifun_calc(output_path, expression, varargin)
```
Defined at source line `1`.

### Description
whifun_calc(output_path, expression, nifti1, nifti2, ...) Calculates a mathematical expression using multiple NIfTI images. Example: whifun_calc('out.nii', 'i1 + i2 + i3', 'sub1.nii', 'sub2.nii', 'sub3.nii') Inputs: output_path : path to save the output NIfTI file expression : expression to evaluate (e.g., 'i1 + i2 - i3') varargin : list of NIfTI image file paths (all in same grid/space) The variables in the expression must be named i1, i2, i3, ... corresponding to the order of NIfTI inputs.

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `output_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `expression` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Uses try/catch; failures are logged, displayed, or returned. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** SPM12
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

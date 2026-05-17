# Module Name: `whifun_functions/whifun_calc.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - whifun_calc(output_path, expression, nifti1, nifti2, ...) Calculates a mathematical expression using multiple NIfTI images. Example: whifun_calc('out.nii', 'i1 + i2 + i3', 'sub1.nii', 'sub2.nii', 'sub3.nii') Inputs: output_path : path to save the output NIfTI file expression : expression to evaluate (e.g., 'i1 + i2 - i3') varargin : list of NIfTI image file paths (all in same grid/space) The variables in the expression must be named i1, i2, i3, ... corresponding to the order of NIfTI inputs.
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: SPM12

## Function: `whifun_calc()`
- **Signature & Definition:** `function whifun_calc(output_path, expression, varargin)` (line 1)
- **Scientific Theory & Formulas:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** whifun_calc(output_path, expression, nifti1, nifti2, ...) Calculates a mathematical expression using multiple NIfTI images. Example: whifun_calc('out.nii', 'i1 + i2 + i3', 'sub1.nii', 'sub2.nii', 'sub3.nii') Inputs: output_path : path to save the output NIfTI file expression : expression to evaluate (e.g., 'i1 + i2 - i3') varargin : list of NIfTI image file paths (all in same grid/space) The variables in the expression must be named i1, i2, i3, ... corresponding to the order of NIfTI inputs.
- **Arguments:**
  - `output_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `expression` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: SPM12
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Uses try/catch; failures are logged, displayed, or returned. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

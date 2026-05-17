# Module Name: `whifun_functions/whifun_preproc_all.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - % ---- input parser ----
  - Internal calls detected: `load_subjects`, `load_subjects_all`, `update_csv`, `whifun_create_fields_preproc`, `whifun_dartel`, `whifun_dartel_normalize_smooth`, `whifun_delete`, `whifun_dir`, `whifun_preproc`, `whifun_qc`, `whifun_save_parameters`, `whifun_update_waitbar`, `write_error`
  - External dependencies detected: MATLAB App Designer, MATLAB table/file I/O, Parallel Computing Toolbox, SPM12, ANTs command-line suite, SLover/MarsBaR-style visualization helpers

## `whifun_preproc_all()`

### Syntax
```matlab
function whifun_preproc_all(output_folder,varargin)
```
Defined at source line `1`.

### Description
% ---- input parser ----

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `output_folder` — character vector or string scalar filesystem path
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
Uses explicit parameter parsing or validation. Defines defaults or branches for optional arguments or missing files. Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands. May pause for interactive user input, which affects batch reproducibility.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `load_subjects`, `load_subjects_all`, `update_csv`, `whifun_create_fields_preproc`, `whifun_dartel`, `whifun_dartel_normalize_smooth`, `whifun_delete`, `whifun_dir`, `whifun_preproc`, `whifun_qc`, `whifun_save_parameters`, `whifun_update_waitbar`, `write_error`
- **External Dependencies:** MATLAB App Designer, MATLAB table/file I/O, Parallel Computing Toolbox, SPM12, ANTs command-line suite, SLover/MarsBaR-style visualization helpers
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects`, `load_subjects_all`, `update_csv`, `whifun_create_fields_preproc`, `whifun_dartel`, `whifun_dartel_normalize_smooth`, `whifun_delete`, `whifun_dir`, `whifun_preproc`, `whifun_qc`, `whifun_save_parameters`, `whifun_update_waitbar`, `write_error`

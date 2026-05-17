# Module Name: `whifun_functions/whifun_preproc_all.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - % ---- input parser ----
  - Internal calls detected: `load_subjects`, `load_subjects_all`, `update_csv`, `whifun_create_fields_preproc`, `whifun_dartel`, `whifun_dartel_normalize_smooth`, `whifun_delete`, `whifun_dir`, `whifun_preproc`, `whifun_qc`, `whifun_save_parameters`, `whifun_update_waitbar`, `write_error`
  - External dependencies detected: MATLAB App Designer, MATLAB table/file I/O, Parallel Computing Toolbox, SPM12, ANTs command-line suite, SLover/MarsBaR-style visualization helpers

## Function: `whifun_preproc_all()`
- **Signature & Definition:** `function whifun_preproc_all(output_folder,varargin)` (line 1)
- **Scientific Theory & Formulas:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** % ---- input parser ----
- **Arguments:**
  - `output_folder` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: `load_subjects`, `load_subjects_all`, `update_csv`, `whifun_create_fields_preproc`, `whifun_dartel`, `whifun_dartel_normalize_smooth`, `whifun_delete`, `whifun_dir`, `whifun_preproc`, `whifun_qc`, `whifun_save_parameters`, `whifun_update_waitbar`, `write_error`
  - External: MATLAB App Designer, MATLAB table/file I/O, Parallel Computing Toolbox, SPM12, ANTs command-line suite, SLover/MarsBaR-style visualization helpers
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Uses explicit parameter parsing or validation. Defines defaults or branches for optional arguments or missing files. Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands. May pause for interactive user input, which affects batch reproducibility.

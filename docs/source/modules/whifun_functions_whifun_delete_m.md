# Module Name: `whifun_functions/whifun_delete.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_DELETE Safely attempts to delete a file. This function wraps the standard MATLAB delete command in a try-catch block. This prevents the pipeline from stopping if a file is locked by the OS, missing, or if permissions are denied. INPUTS: path_ - String or Character array. The full path to the file you wish to remove. EXAMPLE: % Clean up a temporary zipped file after extraction whifun_delete('C:\Data\temp_image.nii.gz'); See also DELETE, TRY, CATCH. Author: Pratik Jain
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_delete()`
- **Signature & Definition:** `function whifun_delete(path_)` (line 1)
- **Scientific Theory & Formulas:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_DELETE Safely attempts to delete a file. This function wraps the standard MATLAB delete command in a try-catch block. This prevents the pipeline from stopping if a file is locked by the OS, missing, or if permissions are denied. INPUTS: path_ - String or Character array. The full path to the file you wish to remove. EXAMPLE: % Clean up a temporary zipped file after extraction whifun_delete('C:\Data\temp_image.nii.gz'); See also DELETE, TRY, CATCH. Author: Pratik Jain
- **Arguments:**
  - `path_` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: `main.mlapp:1656/SelectParticipantsButtonPushed`, `main.mlapp:1774/DataPathTextAreaValueChanged`, `main.mlapp:1895/manuallycoregisterparticipantsButtonPushed`, `main.mlapp:2216/AllfoldersareParticipantsCheckBoxValueChanged`, `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`
- **Edge Cases & Exceptions:** Uses try/catch; failures are logged, displayed, or returned. Emits warnings for recoverable conditions.

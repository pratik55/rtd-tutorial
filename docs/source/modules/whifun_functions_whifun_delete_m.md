# Module Name: `whifun_functions/whifun_delete.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_DELETE Safely attempts to delete a file. This function wraps the standard MATLAB delete command in a try-catch block. This prevents the pipeline from stopping if a file is locked by the OS, missing, or if permissions are denied. INPUTS: path_ - String or Character array. The full path to the file you wish to remove. EXAMPLE: % Clean up a temporary zipped file after extraction whifun_delete('C:\Data\temp_image.nii.gz'); See also DELETE, TRY, CATCH. Author: Pratik Jain
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_delete()`

### Syntax
```matlab
function whifun_delete(path_)
```
Defined at source line `1`.

### Description
WHIFUN_DELETE Safely attempts to delete a file. This function wraps the standard MATLAB delete command in a try-catch block. This prevents the pipeline from stopping if a file is locked by the OS, missing, or if permissions are denied. INPUTS: path_ - String or Character array. The full path to the file you wish to remove. EXAMPLE: % Clean up a temporary zipped file after extraction whifun_delete('C:\Data\temp_image.nii.gz'); See also DELETE, TRY, CATCH. Author: Pratik Jain

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `path_` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Uses try/catch; failures are logged, displayed, or returned. Emits warnings for recoverable conditions.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** `main.mlapp:1656/SelectParticipantsButtonPushed`, `main.mlapp:1774/DataPathTextAreaValueChanged`, `main.mlapp:1895/manuallycoregisterparticipantsButtonPushed`, `main.mlapp:2216/AllfoldersareParticipantsCheckBoxValueChanged`, `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `main.mlapp:1656/SelectParticipantsButtonPushed`, `main.mlapp:1774/DataPathTextAreaValueChanged`, `main.mlapp:1895/manuallycoregisterparticipantsButtonPushed`, `main.mlapp:2216/AllfoldersareParticipantsCheckBoxValueChanged`, `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`

# Module Name: `whifun_functions/whifun_get_datastructure_info.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Key Features:**
  - WHIFUN - Scans subject subfolders (e.g., BAS1, BAS2) for scan completion. 1. Setup subject list
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_get_datastructure_info()`

### Syntax
```matlab
function summary = whifun_get_datastructure_info(dataDir, funcPattern, anatPattern, varargin)
```
Defined at source line `1`.

### Description
WHIFUN - Scans subject subfolders (e.g., BAS1, BAS2) for scan completion. 1. Setup subject list

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `dataDir` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `funcPattern` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `anatPattern` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `summary` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

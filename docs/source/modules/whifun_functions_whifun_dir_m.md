# Module Name: `whifun_functions/whifun_dir.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_DIR Safely retrieves directory information. This function wraps the standard MATLAB dir command in a try-catch block. It is particularly useful for robustly handling missing directories or path-string errors without interrupting the execution of a larger preprocessing loop. INPUTS: path_ - String or Character array. The path or file pattern to be listed (e.g., '/data/sub-*/func/'). OUTPUTS: out - A structure array containing directory information. Returns an empty array [] if the path is invalid or an error occurs. EXAMPLE: % Safely check for the presence of a specific session contents
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_dir()`

### Syntax
```matlab
function out = whifun_dir(path_)
```
Defined at source line `1`.

### Description
WHIFUN_DIR Safely retrieves directory information. This function wraps the standard MATLAB dir command in a try-catch block. It is particularly useful for robustly handling missing directories or path-string errors without interrupting the execution of a larger preprocessing loop. INPUTS: path_ - String or Character array. The path or file pattern to be listed (e.g., '/data/sub-*/func/'). OUTPUTS: out - A structure array containing directory information. Returns an empty array [] if the path is invalid or an error occurs. EXAMPLE: % Safely check for the presence of a specific session contents = whifun_dir(fullfile(subj_dir, 'ses-02')); if isempty(contents) fprintf('Session 02 not found for t

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `path_` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `out` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** `main.mlapp:1656/SelectParticipantsButtonPushed`, `main.mlapp:1774/DataPathTextAreaValueChanged`, `main.mlapp:1895/manuallycoregisterparticipantsButtonPushed`, `main.mlapp:2216/AllfoldersareParticipantsCheckBoxValueChanged`, `main.mlapp:550/ParticipantDatafolderButtonPushed`, `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `main.mlapp:1656/SelectParticipantsButtonPushed`, `main.mlapp:1774/DataPathTextAreaValueChanged`, `main.mlapp:1895/manuallycoregisterparticipantsButtonPushed`, `main.mlapp:2216/AllfoldersareParticipantsCheckBoxValueChanged`, `main.mlapp:550/ParticipantDatafolderButtonPushed`, `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`

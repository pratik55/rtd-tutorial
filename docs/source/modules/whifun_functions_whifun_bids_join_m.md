# Module Name: `whifun_functions/whifun_bids_join.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_BIDS_JOIN Joins multiple strings into an underscore-separated BIDS name. OUT = WHIFUN_BIDS_JOIN(STR1, STR2, ...) takes a variable number of input strings or character arrays and concatenates them using an underscore ('_') delimiter. Empty inputs are automatically ignored. INPUTS: varargin - Any number of string or character array inputs (e.g., 'sub-01', 'ses-pre', 'T1w'). OUTPUTS: out - A single character array of joined elements. EXAMPLE: name = whifun_bids_join('sub-01', 'ses-01', '', 'T1w'); % returns: 'sub-01_ses-01_T1w' See also JOIN, STRING, CHAR. Initialize string array
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_bids_join()`

### Syntax
```matlab
function out = whifun_bids_join(varargin)
```
Defined at source line `1`.

### Description
WHIFUN_BIDS_JOIN Joins multiple strings into an underscore-separated BIDS name. OUT = WHIFUN_BIDS_JOIN(STR1, STR2, ...) takes a variable number of input strings or character arrays and concatenates them using an underscore ('_') delimiter. Empty inputs are automatically ignored. INPUTS: varargin - Any number of string or character array inputs (e.g., 'sub-01', 'ses-pre', 'T1w'). OUTPUTS: out - A single character array of joined elements. EXAMPLE: name = whifun_bids_join('sub-01', 'ses-01', '', 'T1w'); % returns: 'sub-01_ses-01_T1w' See also JOIN, STRING, CHAR. Initialize string array

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `out` — MATLAB value inferred from source usage
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
- **Called By:** `whifun_functions/whifun_post_preproc_fmriprep.m:1/whifun_post_preproc_fmriprep`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `whifun_functions/whifun_post_preproc_fmriprep.m:1/whifun_post_preproc_fmriprep`

# Module Name: `whifun_functions/whifun_parse_bids_filename.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_PARSE_BIDS_FILENAME Extract BIDS/fMRIPrep entities from a filename INPUT fname : string or char OUTPUT info : struct with fields: sub, ses, task, run, space, desc, suffix, extension
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_parse_bids_filename()`

### Syntax
```matlab
function info = whifun_parse_bids_filename(fname)
```
Defined at source line `1`.

### Description
WHIFUN_PARSE_BIDS_FILENAME Extract BIDS/fMRIPrep entities from a filename INPUT fname : string or char OUTPUT info : struct with fields: sub, ses, task, run, space, desc, suffix, extension

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `fname` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `info` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

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

## `extract_entity()`

### Syntax
```matlab
function val = extract_entity(str, key)
```
Defined at source line `38`.

### Description
Extract BIDS entity value (e.g., sub-01 → 01)

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `str` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `key` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `val` — MATLAB value inferred from source usage
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

## `extract_suffix()`

### Syntax
```matlab
function suffix = extract_suffix(str)
```
Defined at source line `52`.

### Description
Extract BIDS suffix (e.g., bold, T1w)

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `str` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `suffix` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

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

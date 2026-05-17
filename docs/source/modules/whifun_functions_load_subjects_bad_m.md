# Module Name: `whifun_functions/load_subjects_bad.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - LOAD_SUBJECTS Loads a list of subjects from a CSV file. [Subj_list, rm] = LOAD_SUBJECTS(folder, name) loads a CSV file named 'name' from the specified 'folder'. It returns a structure array 'Subj_list' containing the subject data and a logical array 'rm' indicating which rows were removed. The function automatically removes subjects marked with 'error', 'motion_ex', or 'manual_ex'. [Subj_list, rm] = LOAD_SUBJECTS(folder, name, first) allows for different behavior on the first run. If 'first' is true (1), the function initializes new 'error' and 'motion_ex' columns with zeros and only removes s
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: MATLAB table/file I/O

## `load_subjects_bad()`

### Syntax
```matlab
function [Subj_list,rm] = load_subjects_bad(folder,name,first)
```
Defined at source line `1`.

### Description
LOAD_SUBJECTS Loads a list of subjects from a CSV file. [Subj_list, rm] = LOAD_SUBJECTS(folder, name) loads a CSV file named 'name' from the specified 'folder'. It returns a structure array 'Subj_list' containing the subject data and a logical array 'rm' indicating which rows were removed. The function automatically removes subjects marked with 'error', 'motion_ex', or 'manual_ex'. [Subj_list, rm] = LOAD_SUBJECTS(folder, name, first) allows for different behavior on the first run. If 'first' is true (1), the function initializes new 'error' and 'motion_ex' columns with zeros and only removes subjects marked with 'manual_ex'. This is useful for initial data processing runs. Input Arguments: f

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `name` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `first` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Subj_list` — structure array containing participant metadata and paths
Output produced by the MATLAB implementation.

#### `rm` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Uses try/catch; failures are logged, displayed, or returned. Handles NaN, Inf, or finite-value filtering. Emits warnings for recoverable conditions.

### Algorithms
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** MATLAB table/file I/O
- **Called By:** `Sub_info.mlapp:161/ParticipantsinerrormotionexmanualexButtonPushed`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `Sub_info.mlapp:161/ParticipantsinerrormotionexmanualexButtonPushed`

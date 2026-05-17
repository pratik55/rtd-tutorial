# Module Name: `whifun_functions/whifun_motion_ex_manual_ex.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$.
- **Key Features:**
  - WHIFUN_MOTION_EX_MANUAL_EX Initializes or validates subject exclusion flags for motion-based or manual exclusion. SUBJ_LIST_1 = WHIFUN_MOTION_EX_MANUAL_EX(SUBJ_LIST_1) This utility function ensures that the `motion_ex` (motion exclusion) and `manual_ex` (manual exclusion) fields exist in the subject structure and are initialized to 0 (meaning the subject is *included*) if they are either missing or empty. It also initializes an `error` flag to 0. Input Arguments: SUBJ_LIST_1 - A scalar structure containing a single subject's information. Must contain the field 'name'. Output Arguments: SUBJ_LI
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_motion_ex_manual_ex()`

### Syntax
```matlab
function Subj_list_1 = whifun_motion_ex_manual_ex(Subj_list_1)
```
Defined at source line `1`.

### Description
WHIFUN_MOTION_EX_MANUAL_EX Initializes or validates subject exclusion flags for motion-based or manual exclusion. SUBJ_LIST_1 = WHIFUN_MOTION_EX_MANUAL_EX(SUBJ_LIST_1) This utility function ensures that the `motion_ex` (motion exclusion) and `manual_ex` (manual exclusion) fields exist in the subject structure and are initialized to 0 (meaning the subject is *included*) if they are either missing or empty. It also initializes an `error` flag to 0. Input Arguments: SUBJ_LIST_1 - A scalar structure containing a single subject's information. Must contain the field 'name'. Output Arguments: SUBJ_LIST_1 - The updated structure with the following fields ensured: - .error: Initialized to 0. - .motio

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `Subj_list_1` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Subj_list_1` — structure array containing participant metadata and paths
Output produced by the MATLAB implementation.

### More About
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

# Module Name: `whifun_functions/whifun_get_common_subjects.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Key Features:**
  - WHIFUN_GET_COMMON_SUBJECTS Returns a structure containing elements whose 'name' field is common between two structure arrays. Inputs: S1, S2 - structure arrays with field 'name' Output: S_common - structure array with common 'name' entries
  - Internal calls detected: `load_subjects_all`
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_get_common_subjects()`

### Syntax
```matlab
function S_common = whifun_get_common_subjects(S1, S2)
```
Defined at source line `1`.

### Description
WHIFUN_GET_COMMON_SUBJECTS Returns a structure containing elements whose 'name' field is common between two structure arrays. Inputs: S1, S2 - structure arrays with field 'name' Output: S_common - structure array with common 'name' entries

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `S1` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `S2` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `S_common` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Extended Capabilities
- **Internal Calls:** `load_subjects_all`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects_all`

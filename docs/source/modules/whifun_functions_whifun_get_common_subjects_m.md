# Module Name: `whifun_functions/whifun_get_common_subjects.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Key Features:**
  - WHIFUN_GET_COMMON_SUBJECTS Returns a structure containing elements whose 'name' field is common between two structure arrays. Inputs: S1, S2 - structure arrays with field 'name' Output: S_common - structure array with common 'name' entries
  - Internal calls detected: `load_subjects_all`
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_get_common_subjects()`
- **Signature & Definition:** `function S_common = whifun_get_common_subjects(S1, S2)` (line 1)
- **Scientific Theory & Formulas:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Functional Purpose:** WHIFUN_GET_COMMON_SUBJECTS Returns a structure containing elements whose 'name' field is common between two structure arrays. Inputs: S1, S2 - structure arrays with field 'name' Output: S_common - structure array with common 'name' entries
- **Arguments:**
  - `S1` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `S2` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `S_common` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `load_subjects_all`
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

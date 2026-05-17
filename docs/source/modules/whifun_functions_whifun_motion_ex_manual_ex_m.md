# Module Name: `whifun_functions/whifun_motion_ex_manual_ex.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$.
- **Key Features:**
  - WHIFUN_MOTION_EX_MANUAL_EX Initializes or validates subject exclusion flags for motion-based or manual exclusion. SUBJ_LIST_1 = WHIFUN_MOTION_EX_MANUAL_EX(SUBJ_LIST_1) This utility function ensures that the `motion_ex` (motion exclusion) and `manual_ex` (manual exclusion) fields exist in the subject structure and are initialized to 0 (meaning the subject is *included*) if they are either missing or empty. It also initializes an `error` flag to 0. Input Arguments: SUBJ_LIST_1 - A scalar structure containing a single subject's information. Must contain the field 'name'. Output Arguments: SUBJ_LI
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_motion_ex_manual_ex()`
- **Signature & Definition:** `function Subj_list_1 = whifun_motion_ex_manual_ex(Subj_list_1)` (line 1)
- **Scientific Theory & Formulas:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$.
- **Functional Purpose:** WHIFUN_MOTION_EX_MANUAL_EX Initializes or validates subject exclusion flags for motion-based or manual exclusion. SUBJ_LIST_1 = WHIFUN_MOTION_EX_MANUAL_EX(SUBJ_LIST_1) This utility function ensures that the `motion_ex` (motion exclusion) and `manual_ex` (manual exclusion) fields exist in the subject structure and are initialized to 0 (meaning the subject is *included*) if they are either missing or empty. It also initializes an `error` flag to 0. Input Arguments: SUBJ_LIST_1 - A scalar structure containing a single subject's information. Must contain the field 'name'. Output Arguments: SUBJ_LIST_1 - The updated structure with the following fields ensured: - .error: Initialized to 0. - .motio
- **Arguments:**
  - `Subj_list_1` (structure array containing participant metadata and paths): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `Subj_list_1` (structure array containing participant metadata and paths): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections.

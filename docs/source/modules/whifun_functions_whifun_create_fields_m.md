# Module Name: `whifun_functions/whifun_create_fields.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Key Features:**
  - WHIFUN_CREATE_FIELDS Adds a set of standard fields to a subject list structure array. Subj_list_all = WHIFUN_CREATE_FIELDS(Subj_list_all) is a utility function that ensures a subject list structure array contains all the necessary fields required for a neuroimaging preprocessing workflow. This function calls an internal helper function `create_field` for a predefined list of fields. If a field does not exist in the structure, it is added to the first element of the array with an empty value. This pre-allocation is a robust way to prepare a subject list for subsequent data storage without throw
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_create_fields()`
- **Signature & Definition:** `function Subj_list_all = whifun_create_fields(Subj_list_all)` (line 1)
- **Scientific Theory & Formulas:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$.
- **Functional Purpose:** WHIFUN_CREATE_FIELDS Adds a set of standard fields to a subject list structure array. Subj_list_all = WHIFUN_CREATE_FIELDS(Subj_list_all) is a utility function that ensures a subject list structure array contains all the necessary fields required for a neuroimaging preprocessing workflow. This function calls an internal helper function `create_field` for a predefined list of fields. If a field does not exist in the structure, it is added to the first element of the array with an empty value. This pre-allocation is a robust way to prepare a subject list for subsequent data storage without throwing errors. The fields added by this function include: - **Exclusion flags**: `error`, `motion_ex`, 
- **Arguments:**
  - `Subj_list_all` (structure array containing participant metadata and paths): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `Subj_list_all` (structure array containing participant metadata and paths): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: `whifun_functions/whifun_check_data.m:1/whifun_check_data`, `whifun_functions/whifun_create_Subj_list.m:1/whifun_create_Subj_list`, `whifun_functions/whifun_create_Subj_list_all_fields.m:1/whifun_create_Subj_list_all_fields`
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `create_field()`
- **Signature & Definition:** `function Subj_list_all = create_field(Subj_list_all,field_)` (line 54)
- **Scientific Theory & Formulas:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Functional Purpose:** WHIFUN_CREATE_FIELDS Adds a set of standard fields to a subject list structure array. Subj_list_all = WHIFUN_CREATE_FIELDS(Subj_list_all) is a utility function that ensures a subject list structure array contains all the necessary fields required for a neuroimaging preprocessing workflow. This function calls an internal helper function `create_field` for a predefined list of fields. If a field does not exist in the structure, it is added to the first element of the array with an empty value. This pre-allocation is a robust way to prepare a subject list for subsequent data storage without throw
- **Arguments:**
  - `Subj_list_all` (structure array containing participant metadata and paths): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `field_` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `Subj_list_all` (structure array containing participant metadata and paths): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

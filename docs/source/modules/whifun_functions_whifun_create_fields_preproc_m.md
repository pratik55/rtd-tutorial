# Module Name: `whifun_functions/whifun_create_fields_preproc.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CREATE_FIELDS_PREPROC Adds preprocessing-specific fields to a subject list. Subj_list_all = WHIFUN_CREATE_FIELDS_PREPROC(Subj_list_all) is a utility function that ensures a subject list structure array contains all the necessary fields for tracking files and data generated during a neuroimaging preprocessing pipeline. This function calls an internal helper function `create_field` for a comprehensive list of fields. If a field does not exist in the structure, it is added to the first element of the array with an empty value. This pre-allocation is a robust way to prepare a subject list f
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_create_fields_preproc()`
- **Signature & Definition:** `function Subj_list_all = whifun_create_fields_preproc(Subj_list_all)` (line 1)
- **Scientific Theory & Formulas:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_CREATE_FIELDS_PREPROC Adds preprocessing-specific fields to a subject list. Subj_list_all = WHIFUN_CREATE_FIELDS_PREPROC(Subj_list_all) is a utility function that ensures a subject list structure array contains all the necessary fields for tracking files and data generated during a neuroimaging preprocessing pipeline. This function calls an internal helper function `create_field` for a comprehensive list of fields. If a field does not exist in the structure, it is added to the first element of the array with an empty value. This pre-allocation is a robust way to prepare a subject list for subsequent data storage without throwing errors. The fields added by this function include: - **F
- **Arguments:**
  - `Subj_list_all` (structure array containing participant metadata and paths): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `Subj_list_all` (structure array containing participant metadata and paths): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `create_field()`
- **Signature & Definition:** `function Subj_list_all = create_field(Subj_list_all,field_)` (line 87)
- **Scientific Theory & Formulas:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_CREATE_FIELDS_PREPROC Adds preprocessing-specific fields to a subject list. Subj_list_all = WHIFUN_CREATE_FIELDS_PREPROC(Subj_list_all) is a utility function that ensures a subject list structure array contains all the necessary fields for tracking files and data generated during a neuroimaging preprocessing pipeline. This function calls an internal helper function `create_field` for a comprehensive list of fields. If a field does not exist in the structure, it is added to the first element of the array with an empty value. This pre-allocation is a robust way to prepare a subject list f
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

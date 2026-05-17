# Module Name: `whifun_functions/whifun_create_fields_preproc.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CREATE_FIELDS_PREPROC Adds preprocessing-specific fields to a subject list. Subj_list_all = WHIFUN_CREATE_FIELDS_PREPROC(Subj_list_all) is a utility function that ensures a subject list structure array contains all the necessary fields for tracking files and data generated during a neuroimaging preprocessing pipeline. This function calls an internal helper function `create_field` for a comprehensive list of fields. If a field does not exist in the structure, it is added to the first element of the array with an empty value. This pre-allocation is a robust way to prepare a subject list f
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_create_fields_preproc()`

### Syntax
```matlab
function Subj_list_all = whifun_create_fields_preproc(Subj_list_all)
```
Defined at source line `1`.

### Description
WHIFUN_CREATE_FIELDS_PREPROC Adds preprocessing-specific fields to a subject list. Subj_list_all = WHIFUN_CREATE_FIELDS_PREPROC(Subj_list_all) is a utility function that ensures a subject list structure array contains all the necessary fields for tracking files and data generated during a neuroimaging preprocessing pipeline. This function calls an internal helper function `create_field` for a comprehensive list of fields. If a field does not exist in the structure, it is added to the first element of the array with an empty value. This pre-allocation is a robust way to prepare a subject list for subsequent data storage without throwing errors. The fields added by this function include: - **F

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `Subj_list_all` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Subj_list_all` — structure array containing participant metadata and paths
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
- **Called By:** `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`

## `create_field()`

### Syntax
```matlab
function Subj_list_all = create_field(Subj_list_all,field_)
```
Defined at source line `87`.

### Description
WHIFUN_CREATE_FIELDS_PREPROC Adds preprocessing-specific fields to a subject list. Subj_list_all = WHIFUN_CREATE_FIELDS_PREPROC(Subj_list_all) is a utility function that ensures a subject list structure array contains all the necessary fields for tracking files and data generated during a neuroimaging preprocessing pipeline. This function calls an internal helper function `create_field` for a comprehensive list of fields. If a field does not exist in the structure, it is added to the first element of the array with an empty value. This pre-allocation is a robust way to prepare a subject list f

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `Subj_list_all` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `field_` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Subj_list_all` — structure array containing participant metadata and paths
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

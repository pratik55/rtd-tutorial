# Module Name: `whifun_functions/whifun_create_fields.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Key Features:**
  - WHIFUN_CREATE_FIELDS Adds a set of standard fields to a subject list structure array. Subj_list_all = WHIFUN_CREATE_FIELDS(Subj_list_all) is a utility function that ensures a subject list structure array contains all the necessary fields required for a neuroimaging preprocessing workflow. This function calls an internal helper function `create_field` for a predefined list of fields. If a field does not exist in the structure, it is added to the first element of the array with an empty value. This pre-allocation is a robust way to prepare a subject list for subsequent data storage without throw
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_create_fields()`

### Syntax
```matlab
function Subj_list_all = whifun_create_fields(Subj_list_all)
```
Defined at source line `1`.

### Description
WHIFUN_CREATE_FIELDS Adds a set of standard fields to a subject list structure array. Subj_list_all = WHIFUN_CREATE_FIELDS(Subj_list_all) is a utility function that ensures a subject list structure array contains all the necessary fields required for a neuroimaging preprocessing workflow. This function calls an internal helper function `create_field` for a predefined list of fields. If a field does not exist in the structure, it is added to the first element of the array with an empty value. This pre-allocation is a robust way to prepare a subject list for subsequent data storage without throwing errors. The fields added by this function include: - **Exclusion flags**: `error`, `motion_ex`,

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
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** `whifun_functions/whifun_check_data.m:1/whifun_check_data`, `whifun_functions/whifun_create_Subj_list.m:1/whifun_create_Subj_list`, `whifun_functions/whifun_create_Subj_list_all_fields.m:1/whifun_create_Subj_list_all_fields`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `whifun_functions/whifun_check_data.m:1/whifun_check_data`, `whifun_functions/whifun_create_Subj_list.m:1/whifun_create_Subj_list`, `whifun_functions/whifun_create_Subj_list_all_fields.m:1/whifun_create_Subj_list_all_fields`

## `create_field()`

### Syntax
```matlab
function Subj_list_all = create_field(Subj_list_all,field_)
```
Defined at source line `54`.

### Description
WHIFUN_CREATE_FIELDS Adds a set of standard fields to a subject list structure array. Subj_list_all = WHIFUN_CREATE_FIELDS(Subj_list_all) is a utility function that ensures a subject list structure array contains all the necessary fields required for a neuroimaging preprocessing workflow. This function calls an internal helper function `create_field` for a predefined list of fields. If a field does not exist in the structure, it is added to the first element of the array with an empty value. This pre-allocation is a robust way to prepare a subject list for subsequent data storage without throw

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
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

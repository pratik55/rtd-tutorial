# Module Name: `whifun_functions/whifun_clean_up_after_preprocessing.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CLEAN_UP_AFTER_PREPROCESSING Manages the deletion of temporary and intermediate files generated during the anatomical and functional preprocessing steps for a single subject. WHIFUN_CLEAN_UP_AFTER_PREPROCESSING(SUBJ_LIST_1, LOG_FILE_ID) This function serves as a wrapper to systematically call a lower-level cleanup function (`whifun_clean_up_folder`) for the main anatomical and functional data directories of a given subject, logging the process. Input Arguments: SUBJ_LIST_1 - A structure containing subject-specific paths, including: - SUBJ_LIST_1.anat_folder: Full path to the subject's a
  - Internal calls detected: `whifun_clean_up_folder`
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_clean_up_after_preprocessing()`

### Syntax
```matlab
function whifun_clean_up_after_preprocessing(Subj_list_1,log_file_id)
```
Defined at source line `1`.

### Description
WHIFUN_CLEAN_UP_AFTER_PREPROCESSING Manages the deletion of temporary and intermediate files generated during the anatomical and functional preprocessing steps for a single subject. WHIFUN_CLEAN_UP_AFTER_PREPROCESSING(SUBJ_LIST_1, LOG_FILE_ID) This function serves as a wrapper to systematically call a lower-level cleanup function (`whifun_clean_up_folder`) for the main anatomical and functional data directories of a given subject, logging the process. Input Arguments: SUBJ_LIST_1 - A structure containing subject-specific paths, including: - SUBJ_LIST_1.anat_folder: Full path to the subject's anatomical data folder. - SUBJ_LIST_1.func_folder: Full path to the subject's functional data folder.

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `Subj_list_1` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `log_file_id` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_clean_up_folder`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_clean_up_folder`

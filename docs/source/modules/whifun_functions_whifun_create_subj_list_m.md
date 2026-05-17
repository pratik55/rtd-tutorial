# Module Name: `whifun_functions/whifun_create_Subj_list.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CREATE_SUBJ_LIST Interactively creates a subject list structure. [Subj_list_all, output_folder] = WHIFUN_CREATE_SUBJ_LIST(output_folder) provides a user-friendly, GUI-based tool for setting up a subject list structure for a preprocessing pipeline. The function guides the user through selecting data, defining patterns for files, and validating the paths for each subject. The function performs the following steps: 1. **Select Folders**: It prompts the user to select an output folder and a main data folder containing all subject directories. 2. **Subject Selection**: It offers options to s
  - Internal calls detected: `my_writetable`, `whifun_create_fields`
  - External dependencies detected: MATLAB App Designer, MATLAB table/file I/O

## `whifun_create_Subj_list()`

### Syntax
```matlab
function [Subj_list_all,output_folder] = whifun_create_Subj_list(output_folder,dataFolder,choice,finalData)
```
Defined at source line `1`.

### Description
WHIFUN_CREATE_SUBJ_LIST Interactively creates a subject list structure. [Subj_list_all, output_folder] = WHIFUN_CREATE_SUBJ_LIST(output_folder) provides a user-friendly, GUI-based tool for setting up a subject list structure for a preprocessing pipeline. The function guides the user through selecting data, defining patterns for files, and validating the paths for each subject. The function performs the following steps: 1. **Select Folders**: It prompts the user to select an output folder and a main data folder containing all subject directories. 2. **Subject Selection**: It offers options to select subjects from the main data folder, either by selecting all, using a wildcard pattern, or manu

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `output_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `dataFolder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `choice` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `finalData` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Subj_list_all` — structure array containing participant metadata and paths
Output produced by the MATLAB implementation.

#### `output_folder` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands. May pause for interactive user input, which affects batch reproducibility.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `my_writetable`, `whifun_create_fields`
- **External Dependencies:** MATLAB App Designer, MATLAB table/file I/O
- **Called By:** `whifun_functions/whifun_create_qc.m:1/whifun_create_qc`, `whifun_functions/whifun_using_other_preproc.m:1/whifun_using_other_preproc`, `whifun_functions/whifun_using_other_preproc_segment_fsl.m:1/whifun_using_other_preproc_segment_fsl`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `my_writetable`, `whifun_create_fields`
- Related callers: `whifun_functions/whifun_create_qc.m:1/whifun_create_qc`, `whifun_functions/whifun_using_other_preproc.m:1/whifun_using_other_preproc`, `whifun_functions/whifun_using_other_preproc_segment_fsl.m:1/whifun_using_other_preproc_segment_fsl`

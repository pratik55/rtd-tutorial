# Module Name: `whifun_functions/whifun_create_Subj_list_all_from_Subj_folder_details.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CREATE_SUBJ_LIST_ALL_FROM_SUBJ_LIST_ALL_DETAILS Scans a directory and creates a subject list if the patterns for the data folder is given. Subj_list_all = WHIFUN_CREATE_SUBJ_LIST_ALL(comm_subj_name, ..., anat_data_name) scans the current directory (or a specified pattern) for subject folders and constructs a list of subject data. It assumes a specific directory structure where each subject has folders for a session, and within that, folders for functional and anatomical data. The function returns a structure array where each element corresponds to a subject and includes paths to their d
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_create_Subj_list_all_from_Subj_folder_details()`

### Syntax
```matlab
function Subj_list_all = whifun_create_Subj_list_all_from_Subj_folder_details(data_path,comm_subj_name,comm_sess_name,func_folder_name,func_data_name,anat_folder_name,anat_data_name)
```
Defined at source line `1`.

### Description
WHIFUN_CREATE_SUBJ_LIST_ALL_FROM_SUBJ_LIST_ALL_DETAILS Scans a directory and creates a subject list if the patterns for the data folder is given. Subj_list_all = WHIFUN_CREATE_SUBJ_LIST_ALL(comm_subj_name, ..., anat_data_name) scans the current directory (or a specified pattern) for subject folders and constructs a list of subject data. It assumes a specific directory structure where each subject has folders for a session, and within that, folders for functional and anatomical data. The function returns a structure array where each element corresponds to a subject and includes paths to their data files. This function is useful for setting up a batch processing script WhiFuN Input Arguments:

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `data_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `comm_subj_name` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `comm_sess_name` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `func_folder_name` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `func_data_name` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `anat_folder_name` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `anat_data_name` — numeric scalar, vector, matrix, or multidimensional array
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
- **Called By:** `main.mlapp:1026/RunDataCheckButtonPushed`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `main.mlapp:1026/RunDataCheckButtonPushed`

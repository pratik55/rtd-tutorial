# Module Name: `whifun_functions/whifun_check_data.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CHECK_DATA Performs an initial, comprehensive check on fMRI and anatomical data files for all subjects in a list, recording key metadata and flagging missing files. [REPORT, N_IMAGE, TR, VOXEL_FUNC, VOXEL_ANAT, MIS_DATA, SUBJ_LIST_ALL] = ... WHIFUN_CHECK_DATA(OUTPUT_FOLDER, SUBJ_LIST_ALL, COMM_SESS_NAME, FUNC_FOLDER_NAME, FUNC_DATA_NAME, ANAT_FOLDER_NAME, ANAT_DATA_NAME, D) This is typically the first step in a neuroimaging pipeline, ensuring all required files exist and have consistent properties before processing begins. Input Arguments: OUTPUT_FOLDER - Path to the directory where the
  - Internal calls detected: `my_writetable`, `whifun_check_data_anat`, `whifun_check_data_func`, `whifun_create_fields`, `whifun_initialise_manual_motion_error_fields`, `whifun_isnan_or_empty`
  - External dependencies detected: MATLAB table/file I/O, ANTs command-line suite

## `whifun_check_data()`

### Syntax
```matlab
function [report,n_image,tr,voxel_func,voxel_anat,mis_data] =  whifun_check_data(output_folder,Subj_list_all,comm_sess_name,func_folder_name,func_data_name,anat_folder_name,anat_data_name,d)
```
Defined at source line `1`.

### Description
WHIFUN_CHECK_DATA Performs an initial, comprehensive check on fMRI and anatomical data files for all subjects in a list, recording key metadata and flagging missing files. [REPORT, N_IMAGE, TR, VOXEL_FUNC, VOXEL_ANAT, MIS_DATA, SUBJ_LIST_ALL] = ... WHIFUN_CHECK_DATA(OUTPUT_FOLDER, SUBJ_LIST_ALL, COMM_SESS_NAME, FUNC_FOLDER_NAME, FUNC_DATA_NAME, ANAT_FOLDER_NAME, ANAT_DATA_NAME, D) This is typically the first step in a neuroimaging pipeline, ensuring all required files exist and have consistent properties before processing begins. Input Arguments: OUTPUT_FOLDER - Path to the directory where the updated subject list CSV will be saved. SUBJ_LIST_ALL - The master structure array containing subje

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `output_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list_all` — structure array containing participant metadata and paths
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

#### `d` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `report` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `n_image` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `tr` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

#### `voxel_func` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

#### `voxel_anat` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

#### `mis_data` — numeric scalar, vector, matrix, or multidimensional array
Output produced by the MATLAB implementation.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Emits warnings for recoverable conditions.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `my_writetable`, `whifun_check_data_anat`, `whifun_check_data_func`, `whifun_create_fields`, `whifun_initialise_manual_motion_error_fields`, `whifun_isnan_or_empty`
- **External Dependencies:** MATLAB table/file I/O, ANTs command-line suite
- **Called By:** `main.mlapp:1026/RunDataCheckButtonPushed`, `whifun_functions/whifun_create_qc.m:1/whifun_create_qc`, `whifun_functions/whifun_using_other_preproc.m:1/whifun_using_other_preproc`, `whifun_functions/whifun_using_other_preproc_segment_fsl.m:1/whifun_using_other_preproc_segment_fsl`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `my_writetable`, `whifun_check_data_anat`, `whifun_check_data_func`, `whifun_create_fields`, `whifun_initialise_manual_motion_error_fields`, `whifun_isnan_or_empty`
- Related callers: `main.mlapp:1026/RunDataCheckButtonPushed`, `whifun_functions/whifun_create_qc.m:1/whifun_create_qc`, `whifun_functions/whifun_using_other_preproc.m:1/whifun_using_other_preproc`, `whifun_functions/whifun_using_other_preproc_segment_fsl.m:1/whifun_using_other_preproc_segment_fsl`

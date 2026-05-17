# Module Name: `whifun_functions/whifun_addpath_and_create_preproc_folders.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_ADDPATH_AND_CREATE_PREPROC_FOLDERS Sets up paths and output directories for preprocessing. quality_control_path = WHIFUN_ADDPATH_AND_CREATE_PREPROC_FOLDERS(preproc_code_path, output_folder) adds necessary code directories to the MATLAB path and creates a standardized set of output folders for storing preprocessing results, quality control metrics, and logs. The function first adds the main preprocessing code path and a subfolder of utility functions to the MATLAB path. It then checks if SPM is available on the path, as it is a critical dependency for most neuroimaging preprocessing pipe
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: SPM12

## `whifun_addpath_and_create_preproc_folders()`

### Syntax
```matlab
function quality_control_path = whifun_addpath_and_create_preproc_folders(preproc_code_path,output_folder)
```
Defined at source line `1`.

### Description
WHIFUN_ADDPATH_AND_CREATE_PREPROC_FOLDERS Sets up paths and output directories for preprocessing. quality_control_path = WHIFUN_ADDPATH_AND_CREATE_PREPROC_FOLDERS(preproc_code_path, output_folder) adds necessary code directories to the MATLAB path and creates a standardized set of output folders for storing preprocessing results, quality control metrics, and logs. The function first adds the main preprocessing code path and a subfolder of utility functions to the MATLAB path. It then checks if SPM is available on the path, as it is a critical dependency for most neuroimaging preprocessing pipelines. If SPM is not found, a message box is displayed to the user. Finally, the function creates a

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `preproc_code_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `output_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `quality_control_path` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** SPM12
- **Called By:** `main.mlapp:1026/RunDataCheckButtonPushed`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `main.mlapp:1026/RunDataCheckButtonPushed`

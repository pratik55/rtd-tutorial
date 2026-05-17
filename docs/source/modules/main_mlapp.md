# Module Name: `main.mlapp`

## Description
- **Module Category:** App Designer GUI module.
- **Theoretical Background:** App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.
- **Key Features:**
  - Properties that correspond to app components
  - Internal calls detected: `BrainNet_MapCfg_WhifuN`, `dice_iou`, `freq_per_band`, `load_subjects`, `load_subjects_all`, `motion_threshold_select`, `my_writetable`, `PCA_regression_parameters`, `rerunpreproc`, `Sub_info`, `Subject_data_folder_details`, `uigetfile_n_dir`, `update_csv`, `whifun_addpath_and_create_preproc_folders`, `whifun_check_data`, `whifun_create_avg_ts`, `whifun_create_fields_preproc`, `whifun_create_file`, `whifun_create_FN_Kmeans`, `whifun_create_FN_Kmeans_WM_GM`, `whifun_create_group_mask`, `whifun_create_Subj_list_all_from_Subj_folder_details`, `whifun_dartel`, `whifun_dartel_normalize_smooth`, `whifun_delete`, `whifun_dir`, `whifun_display_FC`, `whifun_niftiread`, `whifun_plot_data_check_figures`, `whifun_preproc` plus 7 more
  - External dependencies detected: MATLAB App Designer, MATLAB NIfTI I/O, MATLAB table/file I/O, Parallel Computing Toolbox, SPM12, ANTs command-line suite, BrainNet Viewer, SLover/MarsBaR-style visualization helpers

## `main()`

### Syntax
```matlab
classdef main < matlab.apps.AppBase
```
Defined at source line `1`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `main` — MATLAB App or class type
Class definition used to instantiate the module.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Handles NaN, Inf, or finite-value filtering.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** MATLAB App Designer, ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `load_param()`

### Syntax
```matlab
function load_param(app,load_folder,load_name)
```
Defined at source line `204`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `load_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `load_name` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Defines defaults or branches for optional arguments or missing files. Uses try/catch; failures are logged, displayed, or returned.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `load_subjects`
- **External Dependencies:** MATLAB table/file I/O, ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects`

## `load_subjects_dropdown()`

### Syntax
```matlab
function load_subjects_dropdown(app,Subj_list,select_by)
```
Defined at source line `314`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `select_by` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `load_subjects_dropdown2()`

### Syntax
```matlab
function load_subjects_dropdown2(app,Subj_list)
```
Defined at source line `335`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `save_param()`

### Syntax
```matlab
function save_param(app,save_name,save_folder)
```
Defined at source line `347`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `save_name` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `save_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `whifun_save_parameters`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_save_parameters`

## `get_symettry()`

### Syntax
```matlab
function Dice_coef_LR = get_symettry(~,current_clustering_solution)
```
Defined at source line `386`.

### Description
separating the left and right sides of the clustering solutions, and flipping the right side, for whifun_direct comparison to the left

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `~` — unused placeholder
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `current_clustering_solution` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Dice_coef_LR` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `get_symettry_indi()`

### Syntax
```matlab
function Dice_coef_LR = get_symettry_indi(~,current_clustering_solution)
```
Defined at source line `417`.

### Description
separating the left and right sides of the clustering solutions, and flipping the right side, for whifun_direct comparison to the left

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `~` — unused placeholder
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `current_clustering_solution` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Dice_coef_LR` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `dice_iou`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `dice_iou`

## `tooltip()`

### Syntax
```matlab
function tooltip(app)
```
Defined at source line `437`.

### Description
addpaths

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Handles NaN, Inf, or finite-value filtering.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `ParticipantDatafolderButtonPushed()`

### Syntax
```matlab
function ParticipantDatafolderButtonPushed(app, event)
```
Defined at source line `550`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Uses try/catch; failures are logged, displayed, or returned.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `whifun_dir`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_dir`

## `OutputsfolderButtonPushed()`

### Syntax
```matlab
function OutputsfolderButtonPushed(app, event)
```
Defined at source line `582`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Uses try/catch; failures are logged, displayed, or returned.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `SaveParametersButtonPushed()`

### Syntax
```matlab
function SaveParametersButtonPushed(app, event)
```
Defined at source line `593`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Uses try/catch; failures are logged, displayed, or returned.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `LoadParametersButtonPushed()`

### Syntax
```matlab
function LoadParametersButtonPushed(app, event)
```
Defined at source line `604`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Uses try/catch; failures are logged, displayed, or returned.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `RunPreprocessingButtonPushed()`

### Syntax
```matlab
function RunPreprocessingButtonPushed(app, event)
```
Defined at source line `616`.

### Description
% This code written by Pratik Jain. % This code was written with the help of different preprocessing scripts given by % Dr. Xin Di, Dr. Rakibul Hafeez, Dr. Wang Pan, Donna Chen and Wonbum Sohn % Under guidance of Dr Andrew Micheal and Dr. Bharat Biswal. % Defining Important paths and Creating Output whifun_directories

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Defines defaults or branches for optional arguments or missing files. Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands. May pause for interactive user input, which affects batch reproducibility.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `load_subjects`, `load_subjects_all`, `update_csv`, `whifun_create_fields_preproc`, `whifun_dartel`, `whifun_dartel_normalize_smooth`, `whifun_delete`, `whifun_dir`, `whifun_preproc`, `whifun_qc`, `whifun_update_waitbar`, `write_error`
- **External Dependencies:** MATLAB App Designer, MATLAB table/file I/O, Parallel Computing Toolbox, SPM12, ANTs command-line suite, SLover/MarsBaR-style visualization helpers
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects`, `load_subjects_all`, `update_csv`, `whifun_create_fields_preproc`, `whifun_dartel`, `whifun_dartel_normalize_smooth`, `whifun_delete`, `whifun_dir`, `whifun_preproc`, `whifun_qc`, `whifun_update_waitbar`, `write_error`

## `RunDataCheckButtonPushed()`

### Syntax
```matlab
function RunDataCheckButtonPushed(app, event)
```
Defined at source line `1026`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections. May pause for interactive user input, which affects batch reproducibility.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `load_subjects`, `load_subjects_all`, `whifun_addpath_and_create_preproc_folders`, `whifun_check_data`, `whifun_create_Subj_list_all_from_Subj_folder_details`, `whifun_plot_data_check_figures`
- **External Dependencies:** MATLAB App Designer, ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects`, `load_subjects_all`, `whifun_addpath_and_create_preproc_folders`, `whifun_check_data`, `whifun_create_Subj_list_all_from_Subj_folder_details`, `whifun_plot_data_check_figures`

## `BIDSCheckBoxValueChanged()`

### Syntax
```matlab
function BIDSCheckBoxValueChanged(app, event)
```
Defined at source line `1091`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
May pause for interactive user input, which affects batch reproducibility.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `Subject_data_folder_details`
- **External Dependencies:** MATLAB App Designer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `Subject_data_folder_details`

## `NuisanceRegressionDropDownValueChanged()`

### Syntax
```matlab
function NuisanceRegressionDropDownValueChanged(app, event)
```
Defined at source line `1127`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `PCA_regression_parameters`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `PCA_regression_parameters`

## `DisplayFNButtonPushed()`

### Syntax
```matlab
function DisplayFNButtonPushed(app, event)
```
Defined at source line `1145`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections. May pause for interactive user input, which affects batch reproducibility.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `BrainNet_MapCfg_WhifuN`
- **External Dependencies:** MATLAB NIfTI I/O, SPM12, BrainNet Viewer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `BrainNet_MapCfg_WhifuN`

## `DisplayFCButtonPushed()`

### Syntax
```matlab
function DisplayFCButtonPushed(app, event)
```
Defined at source line `1192`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Defines defaults or branches for optional arguments or missing files. Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `whifun_display_FC`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_display_FC`

## `CreateGroupMasksButtonPushed()`

### Syntax
```matlab
function CreateGroupMasksButtonPushed(app, event)
```
Defined at source line `1223`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `load_subjects`, `whifun_create_group_mask`
- **External Dependencies:** MATLAB App Designer, ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects`, `whifun_create_group_mask`

## `WMGroupMaskButtonPushed()`

### Syntax
```matlab
function WMGroupMaskButtonPushed(app, event)
```
Defined at source line `1254`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `whifun_niftiread`
- **External Dependencies:** MATLAB NIfTI I/O, ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_niftiread`

## `WMFNTabButtonDown()`

### Syntax
```matlab
function WMFNTabButtonDown(app, event)
```
Defined at source line `1280`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `whifun_create_file`
- **External Dependencies:** ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_create_file`

## `CreateWMFNButtonPushed()`

### Syntax
```matlab
function CreateWMFNButtonPushed(app, event)
```
Defined at source line `1298`.

### Description
% Clustering WM Functional networks

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections.

### Algorithms
K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `load_subjects`, `whifun_create_FN_Kmeans`
- **External Dependencies:** MATLAB App Designer, ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects`, `whifun_create_FN_Kmeans`

## `GMFNTabButtonDown()`

### Syntax
```matlab
function GMFNTabButtonDown(app, event)
```
Defined at source line `1364`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `whifun_create_file`
- **External Dependencies:** ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_create_file`

## `GMGroupMaskButtonPushed()`

### Syntax
```matlab
function GMGroupMaskButtonPushed(app, event)
```
Defined at source line `1382`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `whifun_niftiread`
- **External Dependencies:** MATLAB NIfTI I/O, ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_niftiread`

## `CreateGMFNButtonPushed()`

### Syntax
```matlab
function CreateGMFNButtonPushed(app, event)
```
Defined at source line `1408`.

### Description
% Clustering GM Functional networks

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `load_subjects`, `whifun_create_FN_Kmeans`
- **External Dependencies:** MATLAB App Designer, ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects`, `whifun_create_FN_Kmeans`

## `StatisticsButtonPushed()`

### Syntax
```matlab
function StatisticsButtonPushed(app, event)
```
Defined at source line `1457`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `load_subjects`, `whifun_statistics`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects`, `whifun_statistics`

## `CompareFNButtonPushed()`

### Syntax
```matlab
function CompareFNButtonPushed(app, event)
```
Defined at source line `1480`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `dice_iou`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `dice_iou`

## `FilterCheckBoxValueChanged()`

### Syntax
```matlab
function FilterCheckBoxValueChanged(app, event)
```
Defined at source line `1515`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `FrequenciesperbandButtonPushed()`

### Syntax
```matlab
function FrequenciesperbandButtonPushed(app, event)
```
Defined at source line `1527`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `freq_per_band`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `freq_per_band`

## `ExtractROITImeseriesButtonPushed()`

### Syntax
```matlab
function ExtractROITImeseriesButtonPushed(app, event)
```
Defined at source line `1538`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Defines defaults or branches for optional arguments or missing files. Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `load_subjects`, `load_subjects_all`, `update_csv`, `whifun_create_avg_ts`
- **External Dependencies:** MATLAB App Designer, ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects`, `load_subjects_all`, `update_csv`, `whifun_create_avg_ts`

## `NetworksAtlasButtonPushed()`

### Syntax
```matlab
function NetworksAtlasButtonPushed(app, event)
```
Defined at source line `1639`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Uses try/catch; failures are logged, displayed, or returned.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `SelectParticipantsButtonPushed()`

### Syntax
```matlab
function SelectParticipantsButtonPushed(app, event)
```
Defined at source line `1656`.

### Description
if ~isempty(app.DataPathTextArea.Value) data_path = app.DataPathTextArea.Value; output_folder = end

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections. May pause for interactive user input, which affects batch reproducibility.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `load_subjects`, `my_writetable`, `uigetfile_n_dir`, `whifun_delete`, `whifun_dir`
- **External Dependencies:** MATLAB table/file I/O, ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects`, `my_writetable`, `uigetfile_n_dir`, `whifun_delete`, `whifun_dir`

## `DataPathTextAreaValueChanged()`

### Syntax
```matlab
function DataPathTextAreaValueChanged(app, event)
```
Defined at source line `1774`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Checks empty arrays, missing files, or empty user selections. May pause for interactive user input, which affects batch reproducibility.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `load_subjects_all`, `whifun_delete`, `whifun_dir`
- **External Dependencies:** ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects_all`, `whifun_delete`, `whifun_dir`

## `QCcheckdoneCheckBoxValueChanged()`

### Syntax
```matlab
function QCcheckdoneCheckBoxValueChanged(app, event)
```
Defined at source line `1831`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `load_subjects`
- **External Dependencies:** ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects`

## `CheckFNSymettryButtonPushed()`

### Syntax
```matlab
function CheckFNSymettryButtonPushed(app, event)
```
Defined at source line `1856`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** MATLAB NIfTI I/O, ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `manuallycoregisterparticipantsButtonPushed()`

### Syntax
```matlab
function manuallycoregisterparticipantsButtonPushed(app, event)
```
Defined at source line `1895`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Checks empty arrays, missing files, or empty user selections. May pause for interactive user input, which affects batch reproducibility.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `load_subjects_all`, `whifun_delete`, `whifun_dir`
- **External Dependencies:** SPM12, ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects_all`, `whifun_delete`, `whifun_dir`

## `DetermineFramewiseDisplacementthresholdsButtonPushed()`

### Syntax
```matlab
function DetermineFramewiseDisplacementthresholdsButtonPushed(app, event)
```
Defined at source line `2138`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `load_subjects_all`, `motion_threshold_select`
- **External Dependencies:** MATLAB App Designer, ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects_all`, `motion_threshold_select`

## `DeletePreprocessingfilesfromaparticularstepButtonPushed()`

### Syntax
```matlab
function DeletePreprocessingfilesfromaparticularstepButtonPushed(app, event)
```
Defined at source line `2169`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `load_subjects_all`, `rerunpreproc`
- **External Dependencies:** ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects_all`, `rerunpreproc`

## `ParticipantsInfoButtonPushed()`

### Syntax
```matlab
function ParticipantsInfoButtonPushed(app, event)
```
Defined at source line `2189`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `Sub_info`
- **External Dependencies:** ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `Sub_info`

## `AllfoldersareParticipantsCheckBoxValueChanged()`

### Syntax
```matlab
function AllfoldersareParticipantsCheckBoxValueChanged(app, event)
```
Defined at source line `2216`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections. May pause for interactive user input, which affects batch reproducibility.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `load_subjects`, `my_writetable`, `uigetfile_n_dir`, `whifun_delete`, `whifun_dir`
- **External Dependencies:** MATLAB table/file I/O, ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects`, `my_writetable`, `uigetfile_n_dir`, `whifun_delete`, `whifun_dir`

## `ManuallyexcludeparticipantsCheckBoxValueChanged()`

### Syntax
```matlab
function ManuallyexcludeparticipantsCheckBoxValueChanged(app, event)
```
Defined at source line `2323`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Checks empty arrays, missing files, or empty user selections. May pause for interactive user input, which affects batch reproducibility.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `load_subjects`, `load_subjects_all`, `uigetfile_n_dir`
- **External Dependencies:** MATLAB table/file I/O, ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects`, `load_subjects_all`, `uigetfile_n_dir`

## `DataPathTextArea_2ValueChanged()`

### Syntax
```matlab
function DataPathTextArea_2ValueChanged(app, event)
```
Defined at source line `2389`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `OverwriteexistingfilesCheckBoxValueChanged()`

### Syntax
```matlab
function OverwriteexistingfilesCheckBoxValueChanged(app, event)
```
Defined at source line `2403`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
May pause for interactive user input, which affects batch reproducibility.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `ParellelProcessingCheckBoxValueChanged()`

### Syntax
```matlab
function ParellelProcessingCheckBoxValueChanged(app, event)
```
Defined at source line `2416`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Uses try/catch; failures are logged, displayed, or returned.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** MATLAB App Designer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `QCviewerButtonPushed()`

### Syntax
```matlab
function QCviewerButtonPushed(app, event)
```
Defined at source line `2449`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `whifun_qcviewer`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_qcviewer`

## `frequencyspecificCheckBoxValueChanged()`

### Syntax
```matlab
function frequencyspecificCheckBoxValueChanged(app, event)
```
Defined at source line `2466`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `CreateWMGMFNButtonPushed()`

### Syntax
```matlab
function CreateWMGMFNButtonPushed(app, event)
```
Defined at source line `2486`.

### Description
% Clustering GM Functional networks

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `load_subjects`, `whifun_create_FN_Kmeans_WM_GM`
- **External Dependencies:** MATLAB App Designer, ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects`, `whifun_create_FN_Kmeans_WM_GM`

## `CheckMaskButtonPushed()`

### Syntax
```matlab
function CheckMaskButtonPushed(app, event)
```
Defined at source line `2534`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `whifun_view`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_view`

## `CheckMaskButton_2Pushed()`

### Syntax
```matlab
function CheckMaskButton_2Pushed(app, event)
```
Defined at source line `2544`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `whifun_view`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_view`

## `CheckatlasButtonPushed()`

### Syntax
```matlab
function CheckatlasButtonPushed(app, event)
```
Defined at source line `2554`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `event` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `whifun_view`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_view`

## `createComponents()`

### Syntax
```matlab
function createComponents(app)
```
Defined at source line `2568`.

### Description
Get the file path for locating images

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Handles NaN, Inf, or finite-value filtering.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `main()`

### Syntax
```matlab
function app = main
```
Defined at source line `3395`.

### Description
Create UIFigure and components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `app` — MATLAB App/UI object or callback handle
Output produced by the MATLAB implementation.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `delete()`

### Syntax
```matlab
function delete(app)
```
Defined at source line `3412`.

### Description
Delete UIFigure when app is deleted

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

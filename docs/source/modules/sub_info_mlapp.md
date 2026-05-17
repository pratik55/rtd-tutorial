# Module Name: `Sub_info.mlapp`

## Description
- **Module Category:** App Designer GUI module.
- **Theoretical Background:** App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.
- **Key Features:**
  - Properties that correspond to app components
  - Internal calls detected: `load_subjects`, `load_subjects_bad`, `my_writetable`
  - External dependencies detected: MATLAB App Designer, MATLAB table/file I/O, ANTs command-line suite

## `Sub_info()`

### Syntax
```matlab
classdef Sub_info < matlab.apps.AppBase
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
#### `Sub_info` — MATLAB App or class type
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
- **Called By:** `main.mlapp:2189/ParticipantsInfoButtonPushed`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `main.mlapp:2189/ParticipantsInfoButtonPushed`

## `load_subjects_all()`

### Syntax
```matlab
function Subj_list_all = load_subjects_all(~,folder,name)
```
Defined at source line `27`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `~` — unused placeholder
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `name` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Subj_list_all` — structure array containing participant metadata and paths
Output produced by the MATLAB implementation.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Uses try/catch; failures are logged, displayed, or returned.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** MATLAB table/file I/O
- **Called By:** `main.mlapp:1026/RunDataCheckButtonPushed`, `main.mlapp:1538/ExtractROITImeseriesButtonPushed`, `main.mlapp:1774/DataPathTextAreaValueChanged`, `main.mlapp:1895/manuallycoregisterparticipantsButtonPushed`, `main.mlapp:2138/DetermineFramewiseDisplacementthresholdsButtonPushed`, `main.mlapp:2169/DeletePreprocessingfilesfromaparticularstepButtonPushed`, `main.mlapp:2323/ManuallyexcludeparticipantsCheckBoxValueChanged`, `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_get_common_subjects.m:1/whifun_get_common_subjects`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`, `whifun_functions/whifun_using_other_preproc.m:1/whifun_using_other_preproc`, `whifun_functions/whifun_using_other_preproc_segment_fsl.m:1/whifun_using_other_preproc_segment_fsl`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `main.mlapp:1026/RunDataCheckButtonPushed`, `main.mlapp:1538/ExtractROITImeseriesButtonPushed`, `main.mlapp:1774/DataPathTextAreaValueChanged`, `main.mlapp:1895/manuallycoregisterparticipantsButtonPushed`, `main.mlapp:2138/DetermineFramewiseDisplacementthresholdsButtonPushed`, `main.mlapp:2169/DeletePreprocessingfilesfromaparticularstepButtonPushed`, `main.mlapp:2323/ManuallyexcludeparticipantsCheckBoxValueChanged`, `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_get_common_subjects.m:1/whifun_get_common_subjects`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`, `whifun_functions/whifun_using_other_preproc.m:1/whifun_using_other_preproc`, `whifun_functions/whifun_using_other_preproc_segment_fsl.m:1/whifun_using_other_preproc_segment_fsl`

## `remove_cols()`

### Syntax
```matlab
function Subj_list_all = remove_cols(~,Subj_list_all)
```
Defined at source line `49`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `~` — unused placeholder
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list_all` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Subj_list_all` — structure array containing participant metadata and paths
Output produced by the MATLAB implementation.

### More About
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Defines defaults or branches for optional arguments or missing files. Uses try/catch; failures are logged, displayed, or returned.

### Algorithms
App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** MATLAB table/file I/O
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `startupFcn()`

### Syntax
```matlab
function startupFcn(app, caller, output_folder, preproc_code_path)
```
Defined at source line `104`.

### Description
Properties that correspond to app components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `app` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `caller` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `output_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `preproc_code_path` — character vector or string scalar filesystem path
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
- **External Dependencies:** ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `AllParticipantsButtonPushed()`

### Syntax
```matlab
function AllParticipantsButtonPushed(app, event)
```
Defined at source line `129`.

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
- **External Dependencies:** ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `ParticipantsgoodtopreprocessButtonPushed()`

### Syntax
```matlab
function ParticipantsgoodtopreprocessButtonPushed(app, event)
```
Defined at source line `142`.

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
- **Internal Calls:** `load_subjects`
- **External Dependencies:** ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects`

## `savechangesButtonPushed()`

### Syntax
```matlab
function savechangesButtonPushed(app, event)
```
Defined at source line `154`.

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
- **Internal Calls:** `my_writetable`
- **External Dependencies:** MATLAB table/file I/O, ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `my_writetable`

## `ParticipantsinerrormotionexmanualexButtonPushed()`

### Syntax
```matlab
function ParticipantsinerrormotionexmanualexButtonPushed(app, event)
```
Defined at source line `161`.

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
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** `load_subjects_bad`
- **External Dependencies:** ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `load_subjects_bad`

## `createComponents()`

### Syntax
```matlab
function createComponents(app)
```
Defined at source line `180`.

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

## `Sub_info()`

### Syntax
```matlab
function app = Sub_info(varargin)
```
Defined at source line `261`.

### Description
Create UIFigure and components

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `app` — MATLAB App/UI object or callback handle
Output produced by the MATLAB implementation.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
Handles NaN, Inf, or finite-value filtering.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** ANTs command-line suite
- **Called By:** `main.mlapp:2189/ParticipantsInfoButtonPushed`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `main.mlapp:2189/ParticipantsInfoButtonPushed`

## `delete()`

### Syntax
```matlab
function delete(app)
```
Defined at source line `278`.

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
Handles NaN, Inf, or finite-value filtering.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

# Module Name: `BrainNetViewer_20191031/BrainNet_MergeMesh.m`

## Description
- **Module Category:** Bundled BrainNetViewer dependency.
- **Theoretical Background:** Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia Function to merge two hemisphere files into one ----------------------------------------------------------- Copyright(c) 2017 State Key Laboratory of Cognitive Neuroscience and Learning, Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.6; Date 20110531; Last edited 20170330 ----------------------------------------------------------- BrainNet_MergeMesh MATLAB code for BrainNet_MergeMesh.fig BrainNet_MergeMesh, by itself, creates a new BrainNet_MergeM
  - Internal calls detected: `findobj`
  - External dependencies detected: MATLAB App Designer, ANTs command-line suite, BrainNet Viewer

## `BrainNet_MergeMesh()`

### Syntax
```matlab
function varargout = BrainNet_MergeMesh(varargin)
```
Defined at source line `1`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia Function to merge two hemisphere files into one ----------------------------------------------------------- Copyright(c) 2017 State Key Laboratory of Cognitive Neuroscience and Learning, Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.6; Date 20110531; Last edited 20170330 ----------------------------------------------------------- BrainNet_MergeMesh MATLAB code for BrainNet_MergeMesh.fig BrainNet_MergeMesh, by itself, creates a new BrainNet_MergeMesh or raises the existing singleton*. H = BrainNet_MergeMesh returns the handle to a new BrainNet_M

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `varargout` — cell array of variable MATLAB arguments
Output produced by the MATLAB implementation.

### More About
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files.

### Algorithms
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** BrainNet Viewer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `BrainNet_MergeMesh_OpeningFcn()`

### Syntax
```matlab
function BrainNet_MergeMesh_OpeningFcn(hObject, eventdata, handles, varargin)
```
Defined at source line `60`.

### Description
This function has no output args, see OutputFcn. hObject handle to figure eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) varargin command line arguments to BrainNet_MergeMesh (see VARARGIN) Choose default command line output for BrainNet_MergeMesh

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hObject` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `eventdata` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `handles` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** `findobj`
- **External Dependencies:** MATLAB App Designer, BrainNet Viewer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `findobj`

## `BrainNet_MergeMesh_OutputFcn()`

### Syntax
```matlab
function varargout = BrainNet_MergeMesh_OutputFcn(hObject, eventdata, handles)
```
Defined at source line `84`.

### Description
varargout cell array for returning output args (see VARARGOUT); hObject handle to figure eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) Get default command line output from handles structure

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hObject` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `eventdata` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `handles` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `varargout` — cell array of variable MATLAB arguments
Output produced by the MATLAB implementation.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** BrainNet Viewer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `OK_button_Callback()`

### Syntax
```matlab
function OK_button_Callback(hObject, eventdata, handles)
```
Defined at source line `95`.

### Description
hObject handle to OK_button (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hObject` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `eventdata` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `handles` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** MATLAB App Designer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `loadpial()`

### Syntax
```matlab
function [vertex, faces, vertex_number, face_number] =loadpial(filename)
```
Defined at source line `120`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia Function to merge two hemisphere files into one ----------------------------------------------------------- Copyright(c) 2017 State Key Laboratory of Cognitive Neuroscience and Learning, Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.6; Date 20110531; Last edited 20170330 ----------------------------------------------------------- BrainNet_MergeMesh MATLAB code for BrainNet_MergeMesh.fig BrainNet_MergeMesh, by itself, creates a new BrainNet_MergeM

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `filename` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `vertex` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `faces` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `vertex_number` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

#### `face_number` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

### More About
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `loadg()`

### Syntax
```matlab
function [vertex, faces, vertex_number, face_number] = loadg(filename)
```
Defined at source line `136`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia Function to merge two hemisphere files into one ----------------------------------------------------------- Copyright(c) 2017 State Key Laboratory of Cognitive Neuroscience and Learning, Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.6; Date 20110531; Last edited 20170330 ----------------------------------------------------------- BrainNet_MergeMesh MATLAB code for BrainNet_MergeMesh.fig BrainNet_MergeMesh, by itself, creates a new BrainNet_MergeM

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `filename` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `vertex` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `faces` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `vertex_number` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

#### `face_number` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

### More About
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `loadobjsurf()`

### Syntax
```matlab
function [vertex, faces, vertex_number, face_number] = loadobjsurf(filename)
```
Defined at source line `147`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia Function to merge two hemisphere files into one ----------------------------------------------------------- Copyright(c) 2017 State Key Laboratory of Cognitive Neuroscience and Learning, Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.6; Date 20110531; Last edited 20170330 ----------------------------------------------------------- BrainNet_MergeMesh MATLAB code for BrainNet_MergeMesh.fig BrainNet_MergeMesh, by itself, creates a new BrainNet_MergeM

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `filename` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `vertex` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `faces` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `vertex_number` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

#### `face_number` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

### More About
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `loadgii()`

### Syntax
```matlab
function [vertex, faces, vertex_number, face_number] = loadgii(filename)
```
Defined at source line `187`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia Function to merge two hemisphere files into one ----------------------------------------------------------- Copyright(c) 2017 State Key Laboratory of Cognitive Neuroscience and Learning, Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.6; Date 20110531; Last edited 20170330 ----------------------------------------------------------- BrainNet_MergeMesh MATLAB code for BrainNet_MergeMesh.fig BrainNet_MergeMesh, by itself, creates a new BrainNet_MergeM

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `filename` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `vertex` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `faces` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `vertex_number` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

#### `face_number` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

### More About
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `loadmz3()`

### Syntax
```matlab
function [vertex, faces, vertex_number, face_number] = loadmz3(filename)
```
Defined at source line `194`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia Function to merge two hemisphere files into one ----------------------------------------------------------- Copyright(c) 2017 State Key Laboratory of Cognitive Neuroscience and Learning, Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.6; Date 20110531; Last edited 20170330 ----------------------------------------------------------- BrainNet_MergeMesh MATLAB code for BrainNet_MergeMesh.fig BrainNet_MergeMesh, by itself, creates a new BrainNet_MergeM

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `filename` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `vertex` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `faces` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `vertex_number` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

#### `face_number` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

### More About
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `loadnv()`

### Syntax
```matlab
function [vertex_number, coord, ntri, tri] = loadnv(filename)
```
Defined at source line `241`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia Function to merge two hemisphere files into one ----------------------------------------------------------- Copyright(c) 2017 State Key Laboratory of Cognitive Neuroscience and Learning, Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.6; Date 20110531; Last edited 20170330 ----------------------------------------------------------- BrainNet_MergeMesh MATLAB code for BrainNet_MergeMesh.fig BrainNet_MergeMesh, by itself, creates a new BrainNet_MergeM

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `filename` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `vertex_number` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

#### `coord` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `ntri` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

#### `tri` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

### More About
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `MergeMesh1()`

### Syntax
```matlab
function MergeMesh1(filename1,filename2,filename3)
```
Defined at source line `250`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia Function to merge two hemisphere files into one ----------------------------------------------------------- Copyright(c) 2017 State Key Laboratory of Cognitive Neuroscience and Learning, Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.6; Date 20110531; Last edited 20170330 ----------------------------------------------------------- BrainNet_MergeMesh MATLAB code for BrainNet_MergeMesh.fig BrainNet_MergeMesh, by itself, creates a new BrainNet_MergeM

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `filename1` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `filename2` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `filename3` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files.

### Algorithms
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `ML_button_Callback()`

### Syntax
```matlab
function ML_button_Callback(hObject, eventdata, handles)
```
Defined at source line `367`.

### Description
hObject handle to ML_button (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) Edited by Mingrui 20120930, add support for nv file.

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hObject` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `eventdata` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `handles` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `ML_edit_Callback()`

### Syntax
```matlab
function ML_edit_Callback(hObject, eventdata, handles)
```
Defined at source line `387`.

### Description
hObject handle to ML_edit (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) Hints: get(hObject,'String') returns contents of ML_edit as text str2double(get(hObject,'String')) returns contents of ML_edit as a double --- Executes during object creation, after setting all properties.

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hObject` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `eventdata` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `handles` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `ML_edit_CreateFcn()`

### Syntax
```matlab
function ML_edit_CreateFcn(hObject, eventdata, handles)
```
Defined at source line `397`.

### Description
hObject handle to ML_edit (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles empty - handles not created until after all CreateFcns called Hint: edit controls usually have a white background on Windows. See ISPC and COMPUTER.

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hObject` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `eventdata` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `handles` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `loadmesh()`

### Syntax
```matlab
function [vertex, faces, vertex_number, faces_number] = loadmesh(filename)
```
Defined at source line `409`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia Function to merge two hemisphere files into one ----------------------------------------------------------- Copyright(c) 2017 State Key Laboratory of Cognitive Neuroscience and Learning, Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.6; Date 20110531; Last edited 20170330 ----------------------------------------------------------- BrainNet_MergeMesh MATLAB code for BrainNet_MergeMesh.fig BrainNet_MergeMesh, by itself, creates a new BrainNet_MergeM

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `filename` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `vertex` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `faces` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `vertex_number` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

#### `faces_number` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

### More About
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `Cancel_button_Callback()`

### Syntax
```matlab
function Cancel_button_Callback(hObject, eventdata, handles)
```
Defined at source line `504`.

### Description
hObject handle to Cancel_button (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hObject` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `eventdata` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `handles` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** `findobj`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `findobj`

## `MR_edit_Callback()`

### Syntax
```matlab
function MR_edit_Callback(hObject, eventdata, handles)
```
Defined at source line `511`.

### Description
hObject handle to MR_edit (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) Hints: get(hObject,'String') returns contents of MR_edit as text str2double(get(hObject,'String')) returns contents of MR_edit as a double --- Executes during object creation, after setting all properties.

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hObject` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `eventdata` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `handles` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `MR_edit_CreateFcn()`

### Syntax
```matlab
function MR_edit_CreateFcn(hObject, eventdata, handles)
```
Defined at source line `521`.

### Description
hObject handle to MR_edit (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles empty - handles not created until after all CreateFcns called Hint: edit controls usually have a white background on Windows. See ISPC and COMPUTER.

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hObject` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `eventdata` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `handles` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `MR_button_Callback()`

### Syntax
```matlab
function MR_button_Callback(hObject, eventdata, handles)
```
Defined at source line `535`.

### Description
hObject handle to MR_button (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) Edited by Mingrui 20120930, add support for nv file.

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hObject` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `eventdata` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `handles` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `Reset_button_Callback()`

### Syntax
```matlab
function Reset_button_Callback(hObject, eventdata, handles)
```
Defined at source line `557`.

### Description
hObject handle to Reset_button (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hObject` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `eventdata` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `handles` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `MN_edit_Callback()`

### Syntax
```matlab
function MN_edit_Callback(hObject, eventdata, handles)
```
Defined at source line `566`.

### Description
hObject handle to MN_edit (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) Hints: get(hObject,'String') returns contents of MN_edit as text str2double(get(hObject,'String')) returns contents of MN_edit as a double --- Executes during object creation, after setting all properties.

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hObject` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `eventdata` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `handles` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `MN_edit_CreateFcn()`

### Syntax
```matlab
function MN_edit_CreateFcn(hObject, eventdata, handles)
```
Defined at source line `576`.

### Description
hObject handle to MN_edit (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles empty - handles not created until after all CreateFcns called Hint: edit controls usually have a white background on Windows. See ISPC and COMPUTER.

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hObject` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `eventdata` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `handles` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `MN_button_Callback()`

### Syntax
```matlab
function MN_button_Callback(hObject, eventdata, handles)
```
Defined at source line `589`.

### Description
hObject handle to MN_button (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hObject` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `eventdata` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `handles` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

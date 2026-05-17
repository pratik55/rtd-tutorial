# Module Name: `BrainNetViewer_20191031/BrainNet_LoadFiles.m`

## Description
- **Module Category:** Bundled BrainNetViewer dependency.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia Function to load files for graph drawing ----------------------------------------------------------- Copyright(c) 2017 State Key Laboratory of Cognitive Neuroscience and Learning, Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.6; Date 20110531; Last edited 20170330 ----------------------------------------------------------- BrainNet_LoadFiles MATLAB code for BrainNet_LoadFiles.fig BrainNet_LoadFiles, by itself, creates a new BrainNet_LoadFiles or
  - Internal calls detected: `coord`, `findobj`
  - External dependencies detected: MATLAB App Designer, MATLAB table/file I/O, SPM12, ANTs command-line suite, BrainNet Viewer

## `BrainNet_LoadFiles()`

### Syntax
```matlab
function varargout = BrainNet_LoadFiles(varargin)
```
Defined at source line `1`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia Function to load files for graph drawing ----------------------------------------------------------- Copyright(c) 2017 State Key Laboratory of Cognitive Neuroscience and Learning, Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.6; Date 20110531; Last edited 20170330 ----------------------------------------------------------- BrainNet_LoadFiles MATLAB code for BrainNet_LoadFiles.fig BrainNet_LoadFiles, by itself, creates a new BrainNet_LoadFiles or raises the existing singleton*. H = BrainNet_LoadFiles returns the handle to a new BrainNet_LoadFile

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
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** BrainNet Viewer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `BrainNet_LoadFiles_OpeningFcn()`

### Syntax
```matlab
function BrainNet_LoadFiles_OpeningFcn(hObject, eventdata, handles, varargin)
```
Defined at source line `62`.

### Description
This function has no output args, see OutputFcn. hObject handle to figure eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) varargin command line arguments to BrainNet_LoadFiles (see VARARGIN) Choose default command line output for BrainNet_LoadFiles

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
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `findobj`
- **External Dependencies:** MATLAB App Designer, BrainNet Viewer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `findobj`

## `BrainNet_LoadFiles_OutputFcn()`

### Syntax
```matlab
function varargout = BrainNet_LoadFiles_OutputFcn(hObject, eventdata, handles)
```
Defined at source line `93`.

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
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

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
Defined at source line `104`.

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
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `findobj`
- **External Dependencies:** MATLAB App Designer, MATLAB table/file I/O
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `findobj`

## `VF_load_a()`

### Syntax
```matlab
function t = VF_load_a(filename)
```
Defined at source line `363`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia Function to load files for graph drawing ----------------------------------------------------------- Copyright(c) 2017 State Key Laboratory of Cognitive Neuroscience and Learning, Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.6; Date 20110531; Last edited 20170330 ----------------------------------------------------------- BrainNet_LoadFiles MATLAB code for BrainNet_LoadFiles.fig BrainNet_LoadFiles, by itself, creates a new BrainNet_LoadFiles or

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `filename` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `t` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Checks empty arrays, missing files, or empty user selections.

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

## `VF_load()`

### Syntax
```matlab
function [hdr,vol]=VF_load(filename)
```
Defined at source line `459`.

### Description
YAN Chao-Gan 111028. Add the path of BrainNet SPM files every time. [BrainNetPath, fileN, extn] = fileparts(which('BrainNet.m'));

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `filename` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `hdr` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `vol` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Emits warnings for recoverable conditions.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** SPM12, BrainNet Viewer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `MF_button_Callback()`

### Syntax
```matlab
function MF_button_Callback(hObject, eventdata, handles)
```
Defined at source line `489`.

### Description
hObject handle to MF_button (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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

## `MF_edit_Callback()`

### Syntax
```matlab
function MF_edit_Callback(hObject, eventdata, handles)
```
Defined at source line `521`.

### Description
hObject handle to MF_edit (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) Hints: get(hObject,'String') returns contents of MF_edit as text str2double(get(hObject,'String')) returns contents of MF_edit as a double --- Executes during object creation, after setting all properties.

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

## `MF_edit_CreateFcn()`

### Syntax
```matlab
function MF_edit_CreateFcn(hObject, eventdata, handles)
```
Defined at source line `531`.

### Description
hObject handle to MF_edit (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles empty - handles not created until after all CreateFcns called Hint: edit controls usually have a white background on Windows. See ISPC and COMPUTER.

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

## `loadpial()`

### Syntax
```matlab
function [vertex, faces, vertex_number, face_number] =loadpial(filename)
```
Defined at source line `542`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia Function to load files for graph drawing ----------------------------------------------------------- Copyright(c) 2017 State Key Laboratory of Cognitive Neuroscience and Learning, Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.6; Date 20110531; Last edited 20170330 ----------------------------------------------------------- BrainNet_LoadFiles MATLAB code for BrainNet_LoadFiles.fig BrainNet_LoadFiles, by itself, creates a new BrainNet_LoadFiles or

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

## `MF_load()`

### Syntax
```matlab
function [vertex_number coord ntri tri]=MF_load(MF)
```
Defined at source line `559`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia Function to load files for graph drawing ----------------------------------------------------------- Copyright(c) 2017 State Key Laboratory of Cognitive Neuroscience and Learning, Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.6; Date 20110531; Last edited 20170330 ----------------------------------------------------------- BrainNet_LoadFiles MATLAB code for BrainNet_LoadFiles.fig BrainNet_LoadFiles, by itself, creates a new BrainNet_LoadFiles or

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `MF` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `vertex_number coord ntri tri` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `coord`
- **External Dependencies:** ANTs command-line suite
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `coord`

## `NI_load()`

### Syntax
```matlab
function [nsph, sphere, label]=NI_load(NI)
```
Defined at source line `764`.

### Description
fid=fopen(NI); i=0; while ~feof(fid) curr=fscanf(fid,'%f',5); if ~isempty(curr) i=i+1; textscan(fid,'%s',1); end end nsph=i; fclose(fid); sphere=zeros(nsph,5); label=cell(nsph,1); fid=fopen(NI); i=0; while ~feof(fid) curr=fscanf(fid,'%f',5); if ~isempty(curr) i=i+1; sphere(i,1:5)=curr; label{i}=textscan(fid,'%s',1); end end fclose(fid); modified by Mingrui 20141028, add support for comments in node file according to Chris Rorden's suggestion

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `NI` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `nsph` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `sphere` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `label` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `NT_load()`

### Syntax
```matlab
function net=NT_load(NT)
```
Defined at source line `799`.

### Description
net=load(NT); modified by Mingrui 20141030, add support for comments in edge file

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `NT` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `net` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** MATLAB table/file I/O
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
Defined at source line `809`.

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
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `findobj`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `findobj`

## `NI_edit_Callback()`

### Syntax
```matlab
function NI_edit_Callback(hObject, eventdata, handles)
```
Defined at source line `818`.

### Description
hObject handle to NI_edit (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) Hints: get(hObject,'String') returns contents of NI_edit as text str2double(get(hObject,'String')) returns contents of NI_edit as a double --- Executes during object creation, after setting all properties.

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

## `NI_edit_CreateFcn()`

### Syntax
```matlab
function NI_edit_CreateFcn(hObject, eventdata, handles)
```
Defined at source line `828`.

### Description
hObject handle to NI_edit (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles empty - handles not created until after all CreateFcns called Hint: edit controls usually have a white background on Windows. See ISPC and COMPUTER.

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

## `NT_edit_Callback()`

### Syntax
```matlab
function NT_edit_Callback(hObject, eventdata, handles)
```
Defined at source line `840`.

### Description
hObject handle to NT_edit (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) Hints: get(hObject,'String') returns contents of NT_edit as text str2double(get(hObject,'String')) returns contents of NT_edit as a double --- Executes during object creation, after setting all properties.

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

## `NT_edit_CreateFcn()`

### Syntax
```matlab
function NT_edit_CreateFcn(hObject, eventdata, handles)
```
Defined at source line `850`.

### Description
hObject handle to NT_edit (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles empty - handles not created until after all CreateFcns called Hint: edit controls usually have a white background on Windows. See ISPC and COMPUTER.

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

## `NI_button_Callback()`

### Syntax
```matlab
function NI_button_Callback(hObject, eventdata, handles)
```
Defined at source line `863`.

### Description
hObject handle to NI_button (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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

## `NT_button_Callback()`

### Syntax
```matlab
function NT_button_Callback(hObject, eventdata, handles)
```
Defined at source line `876`.

### Description
hObject handle to NT_button (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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
Defined at source line `890`.

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

## `NL_edit_Callback()`

### Syntax
```matlab
function NL_edit_Callback(hObject, eventdata, handles)
```
Defined at source line `901`.

### Description
hObject handle to NL_edit (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) Hints: get(hObject,'String') returns contents of NL_edit as text str2double(get(hObject,'String')) returns contents of NL_edit as a double --- Executes during object creation, after setting all properties.

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

## `NL_edit_CreateFcn()`

### Syntax
```matlab
function NL_edit_CreateFcn(hObject, eventdata, handles)
```
Defined at source line `911`.

### Description
hObject handle to NL_edit (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles empty - handles not created until after all CreateFcns called Hint: edit controls usually have a white background on Windows. See ISPC and COMPUTER.

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

## `NL_button_Callback()`

### Syntax
```matlab
function NL_button_Callback(hObject, eventdata, handles)
```
Defined at source line `924`.

### Description
hObject handle to NL_button (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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

## `VF_edit_Callback()`

### Syntax
```matlab
function VF_edit_Callback(hObject, eventdata, handles)
```
Defined at source line `938`.

### Description
hObject handle to VF_edit (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) Hints: get(hObject,'String') returns contents of VF_edit as text str2double(get(hObject,'String')) returns contents of VF_edit as a double --- Executes during object creation, after setting all properties.

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

## `VF_edit_CreateFcn()`

### Syntax
```matlab
function VF_edit_CreateFcn(hObject, eventdata, handles)
```
Defined at source line `948`.

### Description
hObject handle to VF_edit (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles empty - handles not created until after all CreateFcns called Hint: edit controls usually have a white background on Windows. See ISPC and COMPUTER.

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

## `VF_pushbutton_Callback()`

### Syntax
```matlab
function VF_pushbutton_Callback(hObject, eventdata, handles)
```
Defined at source line `961`.

### Description
hObject handle to VF_pushbutton (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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

# Module Name: `BrainNetViewer_20191031/BrainNet.m`

## Description
- **Module Category:** Bundled BrainNetViewer dependency.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('
  - Internal calls detected: `BrainNet_Option`, `findobj`, `vrml`
  - External dependencies detected: MATLAB App Designer, MATLAB table/file I/O, Image Processing Toolbox, BrainNet Viewer

## `BrainNet()`

### Syntax
```matlab
function varargout = BrainNet(varargin)
```
Defined at source line `1`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('CALLBACK',hObject,eventData,handles,...) calls the local function named CALLBACK in BrainNet.M with

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
- **Called By:** `BrainNetViewer_20191031/BrainNet_MapCfg_WhifuN.m:1/BrainNet_MapCfg_WhifuN`, `BrainNetViewer_20191031/BrainNet_MapVolume.m:1/BrainNet_MapVolume`, `BrainNetViewer_20191031/BrainNet_Option.m:82/Initialization`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `BrainNetViewer_20191031/BrainNet_MapCfg_WhifuN.m:1/BrainNet_MapCfg_WhifuN`, `BrainNetViewer_20191031/BrainNet_MapVolume.m:1/BrainNet_MapVolume`, `BrainNetViewer_20191031/BrainNet_Option.m:82/Initialization`

## `BrainNet_OpeningFcn()`

### Syntax
```matlab
function BrainNet_OpeningFcn(hObject, eventdata, handles, varargin)
```
Defined at source line `59`.

### Description
This function has no output args, see OutputFcn. hObject handle to figure eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) varargin command line arguments to BrainNet (see VARARGIN)

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
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** MATLAB App Designer, MATLAB table/file I/O, Image Processing Toolbox, BrainNet Viewer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `BrainNet_OutputFcn()`

### Syntax
```matlab
function varargout = BrainNet_OutputFcn(hObject, eventdata, handles)
```
Defined at source line `346`.

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

## `NV_m_file_Callback()`

### Syntax
```matlab
function NV_m_file_Callback(hObject, eventdata, handles)
```
Defined at source line `357`.

### Description
hObject handle to NV_m_file (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) --------------------------------------------------------------------

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

## `NV_m_exit_Callback()`

### Syntax
```matlab
function NV_m_exit_Callback(hObject, eventdata, handles)
```
Defined at source line `363`.

### Description
hObject handle to NV_m_exit (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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
- **Internal Calls:** `findobj`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `findobj`

## `NV_m_nm_Callback()`

### Syntax
```matlab
function NV_m_nm_Callback(hObject, eventdata, handles)
```
Defined at source line `375`.

### Description
hObject handle to NV_m_nm (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** Image Processing Toolbox, BrainNet Viewer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `NetPrepare()`

### Syntax
```matlab
function NetPrepare
```
Defined at source line `402`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

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

## `NodePrepare()`

### Syntax
```matlab
function NodePrepare
```
Defined at source line `558`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

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

## `ROIPrepare()`

### Syntax
```matlab
function fv = ROIPrepare
```
Defined at source line `635`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `fv` — MATLAB value inferred from source usage
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

## `Nettrans()`

### Syntax
```matlab
function [ncyl,cylinder]=Nettrans(net,t)
```
Defined at source line `700`.

### Description
Modified by Mingrui, 20170309, draw two edges for bidirected edges

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `net` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `t` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `ncyl` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `cylinder` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files.

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

## `CutMesh()`

### Syntax
```matlab
function [t,tl,tr,vl,vr,h1,w1,cut,cuv]=CutMesh(surf)
```
Defined at source line `757`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `t` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

#### `tl` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `tr` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

#### `vl` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `vr` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `h1` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `w1` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `cut` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `cuv` — MATLAB value inferred from source usage
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

## `NoMeshPage()`

### Syntax
```matlab
function w1=NoMeshPage(surf)
```
Defined at source line `782`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `w1` — MATLAB value inferred from source usage
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

## `GenerateView8()`

### Syntax
```matlab
function Viewer=GenerateView8(h1,w1)
```
Defined at source line `787`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `h1` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `w1` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Viewer` — MATLAB value inferred from source usage
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

## `GenerateView6()`

### Syntax
```matlab
function Viewer=GenerateView6(w1)
```
Defined at source line `797`.

### Description
Viewer(1,:)=[0.05,0.58,0.34,0.4,-90,0]; Viewer(2,:)=[0.4,0.58,0.2,0.39,0,90]; Viewer(3,:)=[0.61,0.58,0.34,0.4,180,0]; Viewer(4,:)=[0.05,0.15,0.34,0.4,90,0]; Viewer(5,:)=[0.4,0.15,0.2,0.39,0,-90]; Viewer(6,:)=[0.61,0.15,0.34,0.4,0,0];

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `w1` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Viewer` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

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

## `GenerateView4()`

### Syntax
```matlab
function Viewer=GenerateView4
```
Defined at source line `811`.

### Description
YAN Chao-Gan 111023 Added. For Medium View (4 views)

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Viewer` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

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

## `GenerateView4v()`

### Syntax
```matlab
function Viewer=GenerateView4v
```
Defined at source line `818`.

### Description
Lijie Huang 130221 Added. For Medium View (4 views) and 2 Ventral Views

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Viewer` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

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

## `GenerateView5()`

### Syntax
```matlab
function Viewer = GenerateView5
```
Defined at source line `827`.

### Description
Added by Mingrui, 20170309, add layout for lateral, medial and dorsal view

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Viewer` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

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

## `GenertateSurfM8()`

### Syntax
```matlab
function Surfmatrix=GenertateSurfM8(surf,tl,tr,vl,vr,cuv)
```
Defined at source line `835`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `tl` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `tr` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `vl` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `vr` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `cuv` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Surfmatrix` — numeric scalar, vector, matrix, or multidimensional array
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

## `GenertateSurfM4()`

### Syntax
```matlab
function Surfmatrix=GenertateSurfM4(surf,tl,tr,vl,vr,cuv)
```
Defined at source line `885`.

### Description
YAN Chao-Gan 111023 Added. For Medium View (4 views)

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `tl` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `tr` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `vl` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `vr` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `cuv` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Surfmatrix` — numeric scalar, vector, matrix, or multidimensional array
Output produced by the MATLAB implementation.

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

## `GenertateSurfM4v()`

### Syntax
```matlab
function Surfmatrix=GenertateSurfM4v(surf,tl,tr,vl,vr,cuv)
```
Defined at source line `917`.

### Description
Lijie Huang 130221 Added. For Medium View (4 views) and 2 ventral views

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `tl` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `tr` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `vl` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `vr` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `cuv` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Surfmatrix` — numeric scalar, vector, matrix, or multidimensional array
Output produced by the MATLAB implementation.

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

## `GenertateSurfM5()`

### Syntax
```matlab
function Surfmatrix = GenertateSurfM5(surf,tl,tr,vl,vr,cuv)
```
Defined at source line `958`.

### Description
Added by Mingrui, 20170309, add layout for lateral, medial and dorsal view

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `tl` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `tr` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `vl` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `vr` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `cuv` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Surfmatrix` — numeric scalar, vector, matrix, or multidimensional array
Output produced by the MATLAB implementation.

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

## `PlotMesh4()`

### Syntax
```matlab
function a=PlotMesh4(Viewer,Surfmatrix,alpha)
```
Defined at source line `994`.

### Description
Mingrui Xia 111026 Added. For Medium View (4 views)

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `Viewer` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Surfmatrix` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `alpha` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

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

## `PlotMesh4v()`

### Syntax
```matlab
function a=PlotMesh4v(Viewer,Surfmatrix,alpha)
```
Defined at source line `1039`.

### Description
Mingrui Xia 111026 Added. For Medium View (4 views)

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `Viewer` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Surfmatrix` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `alpha` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

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

## `PlotMesh8()`

### Syntax
```matlab
function a=PlotMesh8(Viewer,Surfmatrix,alpha)
```
Defined at source line `1084`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `Viewer` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Surfmatrix` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `alpha` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
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

## `PlotMesh6()`

### Syntax
```matlab
function a=PlotMesh6(Viewer,surf,alpha)
```
Defined at source line `1128`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `Viewer` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `alpha` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
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

## `PlotMesh1()`

### Syntax
```matlab
function a=PlotMesh1(surf,alpha)
```
Defined at source line `1165`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `alpha` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
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

## `PlotMesh5()`

### Syntax
```matlab
function a = PlotMesh5(Viewer,Surfmatrix,alpha)
```
Defined at source line `1226`.

### Description
Added by Mingrui, 20170309, add layout for lateral, medial and dorsal view

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `Viewer` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Surfmatrix` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `alpha` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

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

## `PlotROI1()`

### Syntax
```matlab
function a = PlotROI1(fv,a,alpha)
```
Defined at source line `1260`.

### Description
Added by Mingrui, 20120529, DrawROI

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `fv` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `a` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `alpha` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

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

## `PlotROI8()`

### Syntax
```matlab
function a = PlotROI8(fv,a,alpha)
```
Defined at source line `1278`.

### Description
Added by Mingrui, 20120529, DrawROI

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `fv` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `a` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `alpha` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

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

## `PlotROI6()`

### Syntax
```matlab
function a = PlotROI6(fv,a,alpha)
```
Defined at source line `1317`.

### Description
Added by Mingrui, 20120529, DrawROI

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `fv` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `a` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `alpha` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

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

## `PlotROI4()`

### Syntax
```matlab
function a = PlotROI4(fv,a,alpha)
```
Defined at source line `1335`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `fv` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `a` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `alpha` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
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

## `PlotROI4v()`

### Syntax
```matlab
function a = PlotROI4v(fv,a,alpha)
```
Defined at source line `1366`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `fv` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `a` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `alpha` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
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

## `PlotROI5()`

### Syntax
```matlab
function a = PlotROI5(fv,a,alpha)
```
Defined at source line `1397`.

### Description
Added by Mingrui, 20170309, add layout for lateral, medial and dorsal view

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `fv` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `a` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `alpha` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

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

## `MapMesh1()`

### Syntax
```matlab
function a=MapMesh1(surf,low,high,alpha)
```
Defined at source line `1436`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `low` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `high` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `alpha` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
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

## `MapMesh8()`

### Syntax
```matlab
function a=MapMesh8(Viewer,Surfmatrix,low,high,alpha)
```
Defined at source line `1484`.

### Description
%% Edited by Mingrui Xia, 20111116, add translucency show

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `Viewer` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Surfmatrix` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `low` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `high` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `alpha` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

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

## `MapMesh4()`

### Syntax
```matlab
function a=MapMesh4(Viewer,Surfmatrix,low,high,alpha)
```
Defined at source line `1533`.

### Description
YAN Chao-Gan 111023 Added. For Medium View (4 views) %% Edited by Mingrui Xia, 20111116, add translucency show

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `Viewer` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Surfmatrix` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `low` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `high` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `alpha` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

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

## `MapMesh4v()`

### Syntax
```matlab
function a=MapMesh4v(Viewer,Surfmatrix,low,high,alpha)
```
Defined at source line `1582`.

### Description
Lijie Huang 130221 Added. For Medium View (4 views) and 2 ventral views %% Edited by Mingrui Xia, 20111116, add translucency show

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `Viewer` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Surfmatrix` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `low` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `high` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `alpha` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

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

## `MapMesh6()`

### Syntax
```matlab
function a=MapMesh6(Viewer,surf,low,high,alpha)
```
Defined at source line `1631`.

### Description
%% Edited by Mingrui Xia, 20111116, add translucency show

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `Viewer` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `low` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `high` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `alpha` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

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

## `MapMesh5()`

### Syntax
```matlab
function a = MapMesh5(Viewer,Surfmatrix,low,high,alpha)
```
Defined at source line `1671`.

### Description
Added by Mingrui, 20170309, add layout for lateral, medial and dorsal view

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `Viewer` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Surfmatrix` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `low` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `high` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `alpha` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

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

## `PlotNode6()`

### Syntax
```matlab
function a=PlotNode6(Viewer,surf,a,n,EC)
```
Defined at source line `1720`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `Viewer` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `a` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `n` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `EC` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
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

## `PlotNode4()`

### Syntax
```matlab
function a=PlotNode4(surf, a, flag, centerX, n, EC)
```
Defined at source line `1855`.

### Description
Mingrui Xia 111026 Added. For Medium View (4 views)

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `a` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `flag` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `centerX` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `n` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `EC` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
Checks empty arrays, missing files, or empty user selections.

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

## `PlotNode4v()`

### Syntax
```matlab
function a=PlotNode4v(surf, a, flag, centerX, n, EC)
```
Defined at source line `2002`.

### Description
Lijie Huang 130221 Added. For Medium View (4 views) and 2 ventral views

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `a` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `flag` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `centerX` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `n` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `EC` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
Checks empty arrays, missing files, or empty user selections.

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

## `PlotNode1()`

### Syntax
```matlab
function a=PlotNode1(surf,a,n,EC)
```
Defined at source line `2149`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `a` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `n` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `EC` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
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

## `PlotNode8()`

### Syntax
```matlab
function PlotNode8(surf,a,flag,centerX,n,EC)
```
Defined at source line `2294`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `a` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `flag` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `centerX` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `n` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `EC` — MATLAB value inferred from source usage
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
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `PlotNode5()`

### Syntax
```matlab
function a = PlotNode5(surf,a,flag,centerX,n,EC)
```
Defined at source line `2461`.

### Description
Added by Mingrui, 20170309, add layout for lateral, medial and dorsal view

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `a` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `flag` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `centerX` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `n` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `EC` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
Checks empty arrays, missing files, or empty user selections.

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

## `PlotLabel6()`

### Syntax
```matlab
function PlotLabel6(surf,i,j)
```
Defined at source line `2630`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `i` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `j` — MATLAB value inferred from source usage
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

## `PlotLabel8()`

### Syntax
```matlab
function PlotLabel8(surf,i,j)
```
Defined at source line `2687`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `i` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `j` — MATLAB value inferred from source usage
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

## `PlotLabel5()`

### Syntax
```matlab
function PlotLabel5(surf,i,j)
```
Defined at source line `2763`.

### Description
Added by Mingrui, 20170309, add layout for lateral, medial and dorsal view

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `i` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `j` — MATLAB value inferred from source usage
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

## `PlotLabel4v()`

### Syntax
```matlab
function PlotLabel4v(surf,i,j)
```
Defined at source line `2796`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `i` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `j` — MATLAB value inferred from source usage
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

## `PlotLabel1()`

### Syntax
```matlab
function PlotLabel1(surf,j)
```
Defined at source line `2825`.

### Description
%% Added by Mingrui Xia, 111028. Plot label for single view. %% Edited by Mingrui Xia, 20111113, label position plus radius times ratio.

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `j` — MATLAB value inferred from source usage
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

## `PlotLabel4()`

### Syntax
```matlab
function PlotLabel4(surf,i,j)
```
Defined at source line `2918`.

### Description
Mingrui Xia 111026 Added. For Medium View (4 views) %% Edited by Mingrui Xia, 20111113, label position plus radius times ratio.

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `i` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `j` — MATLAB value inferred from source usage
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

## `DrawSphere()`

### Syntax
```matlab
function DrawSphere(surf,j,i,n,EC)
```
Defined at source line `2935`.

### Description
switch EC.nod.size case 1 % t=EC.nod.size_size; t = surf.sphere(j,7); case 2 switch EC.nod.size_value case 1 t=surf.sphere(j,7); case 2 if surf.sphere(j,5)<1 t=1; elseif surf.sphere(j,5)>10 t=10; else t=surf.sphere(j,5); end end case 3 if surf.sphere(j,5)>EC.nod.size_threshold switch EC.nod.size_value case 1 t=surf.sphere(j,7); case 2 if surf.sphere(j,5)>10 t=10; else t=surf.sphere(j,5); end end else t=1; end end t=t*EC.nod.size_ratio;

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `j` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `i` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `n` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `EC` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `JudgeNode()`

### Syntax
```matlab
function [centerX,flag]=JudgeNode(surf,vl,vr)
```
Defined at source line `3076`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `vl` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `vr` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `centerX` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `flag` — logical or numeric flag
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

## `PlotLine6()`

### Syntax
```matlab
function PlotLine6(surf,a)
```
Defined at source line `3088`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `a` — MATLAB value inferred from source usage
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

## `PlotLine1()`

### Syntax
```matlab
function PlotLine1(surf)
```
Defined at source line `3128`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
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

## `PlotLine8()`

### Syntax
```matlab
function PlotLine8(surf,a,flag,centerX)
```
Defined at source line `3178`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `a` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `flag` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `centerX` — MATLAB value inferred from source usage
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

## `PlotLine5()`

### Syntax
```matlab
function PlotLine5(surf,a,flag,centerX)
```
Defined at source line `3253`.

### Description
Added by Mingrui, 20170309, add layout for lateral, medial and dorsal view

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `a` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `flag` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `centerX` — MATLAB value inferred from source usage
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

## `PlotLine4()`

### Syntax
```matlab
function PlotLine4(surf,a,flag,centerX)
```
Defined at source line `3324`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `a` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `flag` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `centerX` — MATLAB value inferred from source usage
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

## `PlotLine4v()`

### Syntax
```matlab
function PlotLine4v(surf,a,flag,centerX)
```
Defined at source line `3392`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `a` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `flag` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `centerX` — MATLAB value inferred from source usage
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

## `DrawLine()`

### Syntax
```matlab
function DrawLine(surf,i,nv,iv)
```
Defined at source line `3486`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `surf` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `i` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `nv` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `iv` — MATLAB value inferred from source usage
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
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `DoubleMeshPrepare()`

### Syntax
```matlab
function DoubleMeshPrepare
```
Defined at source line `3864`.

### Description
Added by Mingrui Xia, 20120717, show two brains in one figure

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

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

## `DoubleNodePrepare()`

### Syntax
```matlab
function DoubleNodePrepare
```
Defined at source line `3882`.

### Description
Added by Mingrui Xia, 20120717, show two brains in one figure

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

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

## `BoundaryPrepare()`

### Syntax
```matlab
function BoundaryPrepare
```
Defined at source line `3900`.

### Description
Added by Mingrui, 20190327, draw boundary

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

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

## `FileView()`

### Syntax
```matlab
function a=FileView
```
Defined at source line `3935`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `a` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** MATLAB App Designer, Image Processing Toolbox, BrainNet Viewer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `MapPrepare()`

### Syntax
```matlab
function MapPrepare
```
Defined at source line `4505`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections.

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

## `MapCMPrepare()`

### Syntax
```matlab
function [low high]=MapCMPrepare
```
Defined at source line `4714`.

### Description
BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia ----------------------------------------------------------- Copyright(c) 2019 Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.63; Create Date 20110906; Last edited 20190329 ----------------------------------------------------------- BrainNet MATLAB code for BrainNet.fig BrainNet, by itself, creates a new BrainNet or raises the existing singleton*. H = BrainNet returns the handle to a new BrainNet or the handle to the existing singleton*. BrainNet('

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `low high` — MATLAB value inferred from source usage
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

## `AdjustColorMap()`

### Syntax
```matlab
function NewColorMap=AdjustColorMap(OriginalColorMap,NullColor,NMax,NMin,PMin,PMax)
```
Defined at source line `4853`.

### Description
%% Added by Mingrui Xia, 20111025, to adjust colormap. Adjust the colormap to leave blank to values under threshold, the orginal color map with be set into [NMax NMin] and [PMin PMax]. Written by YAN Chao-Gan, 111023 Input: OriginalColorMap - the original color map NullColor - The values between NMin and PMin will be set to this color (leave blank) NMax, NMin, PMin, PMax - set the axis of colorbar (the orginal color map with be set into [NMax NMin] and [PMin PMax]) Output: NewColorMap - the generated color map, a 1000 by 3 matrix.

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `OriginalColorMap` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `NullColor` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `NMax` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `NMin` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `PMin` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `PMax` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `NewColorMap` — numeric scalar, vector, matrix, or multidimensional array
Output produced by the MATLAB implementation.

### More About
Normalized mutual information is $NMI=\frac{2I(X;Y)}{H(X)+H(Y)}$, where $I(X;Y)=\sum_{ij}p_{ij}\log_2\frac{p_{ij}}{p_i p_j}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Normalized mutual information is $NMI=\frac{2I(X;Y)}{H(X)+H(Y)}$, where $I(X;Y)=\sum_{ij}p_{ij}\log_2\frac{p_{ij}}{p_i p_j}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `NV_m_save_Callback()`

### Syntax
```matlab
function NV_m_save_Callback(hObject, eventdata, handles)
```
Defined at source line `4890`.

### Description
hObject handle to NV_m_save (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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
- **Internal Calls:** `vrml`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `vrml`

## `NV_m_es_Callback()`

### Syntax
```matlab
function NV_m_es_Callback(hObject, eventdata, handles)
```
Defined at source line `4933`.

### Description
hObject handle to NV_m_es (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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
- **External Dependencies:** MATLAB App Designer, BrainNet Viewer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `NV_m_LF_Callback()`

### Syntax
```matlab
function NV_m_LF_Callback(hObject, eventdata, handles)
```
Defined at source line `4962`.

### Description
hObject handle to NV_m_LF (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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
- **External Dependencies:** MATLAB App Designer, BrainNet Viewer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `NV_m_Visualize_Callback()`

### Syntax
```matlab
function NV_m_Visualize_Callback(hObject, eventdata, handles)
```
Defined at source line `4997`.

### Description
hObject handle to NV_m_Visualize (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) --------------------------------------------------------------------

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

## `NV_m_tools_Callback()`

### Syntax
```matlab
function NV_m_tools_Callback(hObject, eventdata, handles)
```
Defined at source line `5003`.

### Description
hObject handle to NV_m_tools (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) --------------------------------------------------------------------

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

## `NV_m_others_Callback()`

### Syntax
```matlab
function NV_m_others_Callback(hObject, eventdata, handles)
```
Defined at source line `5009`.

### Description
hObject handle to NV_m_others (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) --------------------------------------------------------------------

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

## `NV_m_cf_Callback()`

### Syntax
```matlab
function NV_m_cf_Callback(hObject, eventdata, handles)
```
Defined at source line `5015`.

### Description
hObject handle to NV_m_cf (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) global FLAG % Mingrui Xia 111029. For calling from outside. if isfield(FLAG,'IsCalledByREST') && FLAG.IsCalledByREST==1 handles.NV_axes=gca(hObject); end

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
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** Image Processing Toolbox, BrainNet Viewer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `NV_m_mm_Callback()`

### Syntax
```matlab
function NV_m_mm_Callback(hObject, eventdata, handles)
```
Defined at source line `5035`.

### Description
hObject handle to NV_m_mm (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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
- **External Dependencies:** MATLAB App Designer, BrainNet Viewer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `NV_m_help_Callback()`

### Syntax
```matlab
function NV_m_help_Callback(hObject, eventdata, handles)
```
Defined at source line `5043`.

### Description
hObject handle to NV_m_help (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) --------------------------------------------------------------------

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

## `NV_m_about_Callback()`

### Syntax
```matlab
function NV_m_about_Callback(hObject, eventdata, handles)
```
Defined at source line `5049`.

### Description
hObject handle to NV_m_about (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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
- **External Dependencies:** MATLAB App Designer, MATLAB table/file I/O, BrainNet Viewer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `LoadFile_ClickedCallback()`

### Syntax
```matlab
function LoadFile_ClickedCallback(hObject, eventdata, handles)
```
Defined at source line `5125`.

### Description
hObject handle to LoadFile (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** MATLAB App Designer, BrainNet Viewer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `SaveImage_ClickedCallback()`

### Syntax
```matlab
function SaveImage_ClickedCallback(hObject, eventdata, handles)
```
Defined at source line `5166`.

### Description
hObject handle to SaveImage (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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
- **Internal Calls:** `vrml`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `vrml`

## `SagittalView_ClickedCallback()`

### Syntax
```matlab
function SagittalView_ClickedCallback(hObject, eventdata, handles)
```
Defined at source line `5209`.

### Description
hObject handle to SagittalView (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `AxialView_ClickedCallback()`

### Syntax
```matlab
function AxialView_ClickedCallback(hObject, eventdata, handles)
```
Defined at source line `5236`.

### Description
hObject handle to AxialView (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `CoronalView_ClickedCallback()`

### Syntax
```matlab
function CoronalView_ClickedCallback(hObject, eventdata, handles)
```
Defined at source line `5264`.

### Description
hObject handle to CoronalView (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `Presentation_ClickedCallback()`

### Syntax
```matlab
function Presentation_ClickedCallback(hObject, eventdata, handles)
```
Defined at source line `5291`.

### Description
hObject handle to Presentation (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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

## `Stop_ClickedCallback()`

### Syntax
```matlab
function Stop_ClickedCallback(hObject, eventdata, handles)
```
Defined at source line `5307`.

### Description
hObject handle to Stop (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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

## `NV_m_movie_Callback()`

### Syntax
```matlab
function NV_m_movie_Callback(hObject, eventdata, handles)
```
Defined at source line `5315`.

### Description
hObject handle to NV_m_movie (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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

## `NV_m_so_Callback()`

### Syntax
```matlab
function NV_m_so_Callback(hObject, eventdata, handles)
```
Defined at source line `5343`.

### Description
hObject handle to NV_m_so (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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
- **External Dependencies:** MATLAB table/file I/O
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `NV_m_option_Callback()`

### Syntax
```matlab
function NV_m_option_Callback(hObject, eventdata, handles)
```
Defined at source line `5358`.

### Description
hObject handle to NV_m_option (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) --------------------------------------------------------------------

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

## `NV_m_lo_Callback()`

### Syntax
```matlab
function NV_m_lo_Callback(hObject, eventdata, handles)
```
Defined at source line `5364`.

### Description
hObject handle to NV_m_lo (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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
- **Internal Calls:** `BrainNet_Option`
- **External Dependencies:** MATLAB table/file I/O, BrainNet Viewer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `BrainNet_Option`

## `uipushtool3_ClickedCallback()`

### Syntax
```matlab
function uipushtool3_ClickedCallback(hObject, eventdata, handles)
```
Defined at source line `5381`.

### Description
hObject handle to uipushtool3 (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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

## `uitoggletool1_OffCallback()`

### Syntax
```matlab
function uitoggletool1_OffCallback(hObject, eventdata, handles)
```
Defined at source line `5388`.

### Description
hObject handle to uitoggletool1 (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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

## `NV_m_manual_Callback()`

### Syntax
```matlab
function NV_m_manual_Callback(hObject, eventdata, handles)
```
Defined at source line `5398`.

### Description
hObject handle to NV_m_manual (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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
Defines defaults or branches for optional arguments or missing files.

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

## `NV_m_ColormapEditor_Callback()`

### Syntax
```matlab
function NV_m_ColormapEditor_Callback(hObject, eventdata, handles)
```
Defined at source line `5409`.

### Description
hObject handle to NV_m_ColormapEditor (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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

## `NV_m_ApplyColormap_Callback()`

### Syntax
```matlab
function NV_m_ApplyColormap_Callback(hObject, eventdata, handles)
```
Defined at source line `5416`.

### Description
hObject handle to NV_m_ApplyColormap (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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

## `uitoggletool5_ClickedCallback()`

### Syntax
```matlab
function uitoggletool5_ClickedCallback(hObject, eventdata, handles)
```
Defined at source line `5432`.

### Description
hObject handle to uitoggletool5 (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) --- Executes during object deletion, before destroying properties.

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

## `NV_fig_DeleteFcn()`

### Syntax
```matlab
function NV_fig_DeleteFcn(hObject, eventdata, handles)
```
Defined at source line `5438`.

### Description
hObject handle to NV_fig (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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
- **External Dependencies:** BrainNet Viewer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `NV_m_SaveColormap_Callback()`

### Syntax
```matlab
function NV_m_SaveColormap_Callback(hObject, eventdata, handles)
```
Defined at source line `5449`.

### Description
hObject handle to NV_m_SaveColormap (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) %% Added by Mingrui Xia, 20120710 save current colormap

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

## `MV_m_ViewMatrix_Callback()`

### Syntax
```matlab
function MV_m_ViewMatrix_Callback(hObject, eventdata, handles)
```
Defined at source line `5470`.

### Description
hObject handle to MV_m_ViewMatrix (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `NV_t_ViewMatrix_ClickedCallback()`

### Syntax
```matlab
function NV_t_ViewMatrix_ClickedCallback(hObject, eventdata, handles)
```
Defined at source line `5483`.

### Description
hObject handle to NV_t_ViewMatrix (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `NV_menu_saveboundary_Callback()`

### Syntax
```matlab
function NV_menu_saveboundary_Callback(hObject, eventdata, handles)
```
Defined at source line `5497`.

### Description
hObject handle to NV_menu_saveboundary (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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

## `PlotEdit_toggle_ClickedCallback()`

### Syntax
```matlab
function PlotEdit_toggle_ClickedCallback(hObject, eventdata, handles)
```
Defined at source line `5522`.

### Description
hObject handle to PlotEdit_toggle (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA) --------------------------------------------------------------------

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

## `PlotEdit_toggle_OffCallback()`

### Syntax
```matlab
function PlotEdit_toggle_OffCallback(hObject, eventdata, handles)
```
Defined at source line `5530`.

### Description
hObject handle to PlotEdit_toggle (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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

## `PlotEdit_toggle_OnCallback()`

### Syntax
```matlab
function PlotEdit_toggle_OnCallback(hObject, eventdata, handles)
```
Defined at source line `5538`.

### Description
hObject handle to PlotEdit_toggle (see GCBO) eventdata reserved - to be defined in a future version of MATLAB handles structure with handles and user data (see GUIDATA)

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

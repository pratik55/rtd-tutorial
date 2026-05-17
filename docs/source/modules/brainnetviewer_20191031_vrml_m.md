# Module Name: `BrainNetViewer_20191031/vrml.m`

## Description
- **Module Category:** Bundled BrainNetViewer dependency.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are
  - Internal calls detected: `findobj`
  - External dependencies detected: ANTs command-line suite

## `vrml()`

### Syntax
```matlab
function vrml(h, filename, opts)
```
Defined at source line `1`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are not implemented by the viewers. Others are due to features not implemented by vrml.m. In some cases

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `h` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `filename` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `opts` — numeric time-series matrix, commonly T x R, V x T, or T x R x S
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Uses try/catch; failures are logged, displayed, or returned. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** ANTs command-line suite
- **Called By:** `BrainNetViewer_20191031/BrainNet.m:4890/NV_m_save_Callback`, `BrainNetViewer_20191031/BrainNet.m:5166/SaveImage_ClickedCallback`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `BrainNetViewer_20191031/BrainNet.m:4890/NV_m_save_Callback`, `BrainNetViewer_20191031/BrainNet.m:5166/SaveImage_ClickedCallback`

## `WriteFileHeaderAndInfo()`

### Syntax
```matlab
function WriteFileHeaderAndInfo()
```
Defined at source line `80`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

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
Handles NaN, Inf, or finite-value filtering.

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

## `ProcessObject()`

### Syntax
```matlab
function ProcessObject(obj_handle, opts)
```
Defined at source line `88`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj_handle` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `opts` — numeric time-series matrix, commonly T x R, V x T, or T x R x S
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

## `HandleFigure()`

### Syntax
```matlab
function HandleFigure(obj,opts)
```
Defined at source line `101`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `opts` — numeric time-series matrix, commonly T x R, V x T, or T x R x S
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

## `HandleAxes()`

### Syntax
```matlab
function HandleAxes(obj_handle, opts)
```
Defined at source line `111`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj_handle` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `opts` — numeric time-series matrix, commonly T x R, V x T, or T x R x S
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
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `findobj`

## `HandleLight()`

### Syntax
```matlab
function HandleLight(obj)
```
Defined at source line `162`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

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

## `HandleText()`

### Syntax
```matlab
function HandleText(obj)
```
Defined at source line `181`.

### Description
check to see what kind of object we received a real HG object or maybe just a label of the axis.

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
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

## `HandlePatch()`

### Syntax
```matlab
function HandlePatch(obj_handle,opts)
```
Defined at source line `212`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj_handle` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `opts` — numeric time-series matrix, commonly T x R, V x T, or T x R x S
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

## `HandleSurface()`

### Syntax
```matlab
function HandleSurface(obj_handle, opts)
```
Defined at source line `219`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj_handle` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `opts` — numeric time-series matrix, commonly T x R, V x T, or T x R x S
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

## `HandlePatch_SurfaceObjs()`

### Syntax
```matlab
function HandlePatch_SurfaceObjs(obj_handle,info,opts)
```
Defined at source line `226`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj_handle` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `info` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `opts` — numeric time-series matrix, commonly T x R, V x T, or T x R x S
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

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

## `HandleLine()`

### Syntax
```matlab
function HandleLine(obj)
```
Defined at source line `289`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
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

## `HandleImage()`

### Syntax
```matlab
function HandleImage(obj)
```
Defined at source line `299`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
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

## `BeginShape()`

### Syntax
```matlab
function BeginShape(type)
```
Defined at source line `326`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `type` — character vector, string scalar, or categorical option
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

## `EndShape()`

### Syntax
```matlab
function EndShape
```
Defined at source line `334`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

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

## `color()`

### Syntax
```matlab
function color(hgObj,fcn,type)
```
Defined at source line `340`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hgObj` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `fcn` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `type` — character vector, string scalar, or categorical option
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

## `facecolor()`

### Syntax
```matlab
function facecolor(hgObj,fcn,type)
```
Defined at source line `354`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hgObj` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `fcn` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `type` — character vector, string scalar, or categorical option
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

## `coord()`

### Syntax
```matlab
function coord(hgObj,fcn,name,usage)
```
Defined at source line `367`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hgObj` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `fcn` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `name` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `usage` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** `BrainNetViewer_20191031/BrainNet_GenCoord.m:1/BrainNet_GenCoord`, `BrainNetViewer_20191031/BrainNet_LoadFiles.m:559/MF_load`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `BrainNetViewer_20191031/BrainNet_GenCoord.m:1/BrainNet_GenCoord`, `BrainNetViewer_20191031/BrainNet_LoadFiles.m:559/MF_load`

## `coordIndex()`

### Syntax
```matlab
function coordIndex(hgObj,fcn)
```
Defined at source line `386`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hgObj` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `fcn` — MATLAB value inferred from source usage
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

## `colorIndex()`

### Syntax
```matlab
function colorIndex(hgObj,fcn,type)
```
Defined at source line `393`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hgObj` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `fcn` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `type` — character vector, string scalar, or categorical option
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

## `texture()`

### Syntax
```matlab
function texture(hgObj)
```
Defined at source line `398`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hgObj` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

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

## `surfColor()`

### Syntax
```matlab
function surfColor(obj) %#ok<*DEFNU>
```
Defined at source line `418`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

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
Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

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

## `patchColor()`

### Syntax
```matlab
function patchColor(obj) %#ok<*DEFNU>
```
Defined at source line `425`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

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
Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

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

## `surfCoordIndex()`

### Syntax
```matlab
function surfCoordIndex(obj)
```
Defined at source line `437`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
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

## `patchCoordIndex()`

### Syntax
```matlab
function patchCoordIndex(obj)
```
Defined at source line `446`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
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

## `patchColorIndex()`

### Syntax
```matlab
function patchColorIndex(obj,type)
```
Defined at source line `453`.

### Description
n determines index/true coloring

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `type` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

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

## `surfColorIndex()`

### Syntax
```matlab
function surfColorIndex(obj,type)
```
Defined at source line `473`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `type` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

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

## `lineCoord()`

### Syntax
```matlab
function lineCoord(obj)
```
Defined at source line `498`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
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

## `lineCoordIndex()`

### Syntax
```matlab
function lineCoordIndex(obj)
```
Defined at source line `509`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
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

## `surfCoord()`

### Syntax
```matlab
function surfCoord(obj)
```
Defined at source line `516`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
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

## `patchCoord()`

### Syntax
```matlab
function patchCoord(obj)
```
Defined at source line `525`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
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

## `axesTickCoord()`

### Syntax
```matlab
function axesTickCoord(obj)
```
Defined at source line `532`.

### Description
XTICK

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
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

## `axesTickCoordIndex()`

### Syntax
```matlab
function axesTickCoordIndex(obj)
```
Defined at source line `557`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
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

## `outputAxesCube()`

### Syntax
```matlab
function outputAxesCube(obj)
```
Defined at source line `584`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
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

## `outputAxesTickLabels()`

### Syntax
```matlab
function outputAxesTickLabels(obj)
```
Defined at source line `608`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
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

## `outputAxesTicks()`

### Syntax
```matlab
function outputAxesTicks(obj)
```
Defined at source line `626`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
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

## `outputColormap()`

### Syntax
```matlab
function outputColormap(cmap)
```
Defined at source line `632`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `cmap` — numeric scalar, vector, matrix, or multidimensional array
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

## `colorMapping()`

### Syntax
```matlab
function rdata = colorMapping(data, clim, colormap_length, mapping_type)
```
Defined at source line `635`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `data` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `clim` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `colormap_length` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `mapping_type` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `rdata` — numeric scalar, vector, matrix, or multidimensional array
Output produced by the MATLAB implementation.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

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

## `sendStr()`

### Syntax
```matlab
function sendStr(indent,str)
```
Defined at source line `652`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `indent` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `str` — numeric scalar or numeric vector
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

## `outputOtherViewpoints()`

### Syntax
```matlab
function outputOtherViewpoints(obj)
```
Defined at source line `659`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
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

## `computeOrientation()`

### Syntax
```matlab
function o = computeOrientation(T)
```
Defined at source line `669`.

### Description
VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `T` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `o` — MATLAB value inferred from source usage
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

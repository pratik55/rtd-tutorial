# Module Name: `BrainNetViewer_20191031/vrml.m`
- **Module Category:** Bundled BrainNetViewer dependency.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
  - Internal calls detected: `findobj`
  - External dependencies detected: ANTs command-line suite

## Function: `vrml()`
- **Signature & Definition:** `function vrml(h, filename, opts)` (line 1)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are not implemented by the viewers. Others are due to features not implemented by vrml.m. In some cases 
- **Arguments:**
  - `h` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `filename` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `opts` (numeric time-series matrix, commonly T x R, V x T, or T x R x S): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: ANTs command-line suite
  - Called By: `BrainNetViewer_20191031/BrainNet.m:4890/NV_m_save_Callback`, `BrainNetViewer_20191031/BrainNet.m:5166/SaveImage_ClickedCallback`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Uses try/catch; failures are logged, displayed, or returned. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

## Function: `WriteFileHeaderAndInfo()`
- **Signature & Definition:** `function WriteFileHeaderAndInfo()` (line 80)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - No explicit input arguments.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Handles NaN, Inf, or finite-value filtering.

## Function: `ProcessObject()`
- **Signature & Definition:** `function ProcessObject(obj_handle, opts)` (line 88)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj_handle` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `opts` (numeric time-series matrix, commonly T x R, V x T, or T x R x S): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `HandleFigure()`
- **Signature & Definition:** `function HandleFigure(obj,opts)` (line 101)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `opts` (numeric time-series matrix, commonly T x R, V x T, or T x R x S): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `HandleAxes()`
- **Signature & Definition:** `function HandleAxes(obj_handle, opts)` (line 111)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj_handle` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `opts` (numeric time-series matrix, commonly T x R, V x T, or T x R x S): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: `findobj`
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections.

## Function: `HandleLight()`
- **Signature & Definition:** `function HandleLight(obj)` (line 162)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

## Function: `HandleText()`
- **Signature & Definition:** `function HandleText(obj)` (line 181)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** check to see what kind of object we received a real HG object or maybe just a label of the axis.
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `HandlePatch()`
- **Signature & Definition:** `function HandlePatch(obj_handle,opts)` (line 212)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj_handle` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `opts` (numeric time-series matrix, commonly T x R, V x T, or T x R x S): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `HandleSurface()`
- **Signature & Definition:** `function HandleSurface(obj_handle, opts)` (line 219)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj_handle` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `opts` (numeric time-series matrix, commonly T x R, V x T, or T x R x S): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `HandlePatch_SurfaceObjs()`
- **Signature & Definition:** `function HandlePatch_SurfaceObjs(obj_handle,info,opts)` (line 226)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj_handle` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `info` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `opts` (numeric time-series matrix, commonly T x R, V x T, or T x R x S): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

## Function: `HandleLine()`
- **Signature & Definition:** `function HandleLine(obj)` (line 289)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `HandleImage()`
- **Signature & Definition:** `function HandleImage(obj)` (line 299)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `BeginShape()`
- **Signature & Definition:** `function BeginShape(type)` (line 326)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `type` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `EndShape()`
- **Signature & Definition:** `function EndShape` (line 334)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - No explicit input arguments.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `color()`
- **Signature & Definition:** `function color(hgObj,fcn,type)` (line 340)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `hgObj` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `fcn` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `type` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `facecolor()`
- **Signature & Definition:** `function facecolor(hgObj,fcn,type)` (line 354)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `hgObj` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `fcn` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `type` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `coord()`
- **Signature & Definition:** `function coord(hgObj,fcn,name,usage)` (line 367)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `hgObj` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `fcn` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `name` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `usage` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: `BrainNetViewer_20191031/BrainNet_GenCoord.m:1/BrainNet_GenCoord`, `BrainNetViewer_20191031/BrainNet_LoadFiles.m:559/MF_load`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files.

## Function: `coordIndex()`
- **Signature & Definition:** `function coordIndex(hgObj,fcn)` (line 386)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `hgObj` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `fcn` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `colorIndex()`
- **Signature & Definition:** `function colorIndex(hgObj,fcn,type)` (line 393)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `hgObj` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `fcn` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `type` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `texture()`
- **Signature & Definition:** `function texture(hgObj)` (line 398)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `hgObj` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

## Function: `surfColor()`
- **Signature & Definition:** `function surfColor(obj) %#ok<*DEFNU>` (line 418)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - No explicit input arguments.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

## Function: `patchColor()`
- **Signature & Definition:** `function patchColor(obj) %#ok<*DEFNU>` (line 425)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - No explicit input arguments.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

## Function: `surfCoordIndex()`
- **Signature & Definition:** `function surfCoordIndex(obj)` (line 437)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `patchCoordIndex()`
- **Signature & Definition:** `function patchCoordIndex(obj)` (line 446)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `patchColorIndex()`
- **Signature & Definition:** `function patchColorIndex(obj,type)` (line 453)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** n determines index/true coloring
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `type` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

## Function: `surfColorIndex()`
- **Signature & Definition:** `function surfColorIndex(obj,type)` (line 473)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `type` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

## Function: `lineCoord()`
- **Signature & Definition:** `function lineCoord(obj)` (line 498)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections.

## Function: `lineCoordIndex()`
- **Signature & Definition:** `function lineCoordIndex(obj)` (line 509)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `surfCoord()`
- **Signature & Definition:** `function surfCoord(obj)` (line 516)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `patchCoord()`
- **Signature & Definition:** `function patchCoord(obj)` (line 525)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `axesTickCoord()`
- **Signature & Definition:** `function axesTickCoord(obj)` (line 532)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** XTICK
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `axesTickCoordIndex()`
- **Signature & Definition:** `function axesTickCoordIndex(obj)` (line 557)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `outputAxesCube()`
- **Signature & Definition:** `function outputAxesCube(obj)` (line 584)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `outputAxesTickLabels()`
- **Signature & Definition:** `function outputAxesTickLabels(obj)` (line 608)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `outputAxesTicks()`
- **Signature & Definition:** `function outputAxesTicks(obj)` (line 626)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `outputColormap()`
- **Signature & Definition:** `function outputColormap(cmap)` (line 632)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `cmap` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `colorMapping()`
- **Signature & Definition:** `function rdata = colorMapping(data, clim, colormap_length, mapping_type)` (line 635)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `data` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `clim` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `colormap_length` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `mapping_type` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `rdata` (numeric scalar, vector, matrix, or multidimensional array): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

## Function: `sendStr()`
- **Signature & Definition:** `function sendStr(indent,str)` (line 652)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `indent` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `str` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `outputOtherViewpoints()`
- **Signature & Definition:** `function outputOtherViewpoints(obj)` (line 659)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `computeOrientation()`
- **Signature & Definition:** `function o = computeOrientation(T)` (line 669)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** VRML Save graphics to VRML 97 file. VRML(H, FILENAME) saves a VRML 97 file containing the object with handle H and its descendants. If the FILENAME does not include an extension, ".wrl" is appended. If a file with the name FILENAME exists, it is overwritten. VRML(H) saves H and its descendants to the file "matlab.wrl". VRML(H, FILENAME, 'noedgelines') saves the object so that any edge lines of Patch objects are not saved in the resulting VRML file. Note that there are rendering differences between MATLAB and the VRML viewers. Some of these differences are due to VRML 97 spec features that are 
- **Arguments:**
  - `T` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `o` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

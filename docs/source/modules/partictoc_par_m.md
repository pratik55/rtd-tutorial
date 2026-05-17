# Module Name: `parTicToc/Par.m`

## Description
- **Module Category:** Bundled parallel timing helper.
- **Theoretical Background:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: Parallel Computing Toolbox

## `Par()`

### Syntax
```matlab
classdef Par < handle
```
Defined at source line `1`.

### Description
Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR measurements StartTime - Return the start time of the measurement StopTime - Return the stop time of

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Par` — MATLAB App or class type
Class definition used to instantiate the module.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** Parallel Computing Toolbox
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `Par()`

### Syntax
```matlab
function obj = Par(n, varargin)
```
Defined at source line `81`.

### Description
PAR Contructor for the Par object obj = Par(N) Creates an array of loop timer object for PARFOR loops. N is a positive integer equal to the length of iterations in the PARFOR loop. Special case used internally check first since we want this to happen immediately.

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `n` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `obj` — MATLAB App/UI object or callback handle
Output produced by the MATLAB implementation.

### More About
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Tips
Defines defaults or branches for optional arguments or missing files. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** Parallel Computing Toolbox
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `horzcat()`

### Syntax
```matlab
function newobj = horzcat(varargin)
```
Defined at source line `122`.

### Description
HORZCAT Horizontally concatenate multiple PARFOR measurements. horzcat(p1, p2, ...) or [p1, p2, ...] Concatenates multiple Par objects. This allows you to combine results from multiple PARFOR blocks that are run sequentially. P1, P2, ... must be either Par objects or an empty array ([]).

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `newobj` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Tips
Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** Parallel Computing Toolbox
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `stop()`

### Syntax
```matlab
function stop(obj)
```
Defined at source line `171`.

### Description
STOP Stop the measurement. obj.stop() or stop(obj) Stops the measurement process. This should be called right after the parfor loop.

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
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Tips
Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** Parallel Computing Toolbox
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `StartTime()`

### Syntax
```matlab
function val = StartTime(obj)
```
Defined at source line `189`.

### Description
STARTTIME Return the end time of the measurement. val = obj.StartTime() or val = StartTime(obj) Returns the start time relative to the initial creation of the object. Usually, this is zero. If this object was a concatenation of multiple Par objects, then this will return multiple start times for each of the objects, relative to the initial start time. The start time is stored in the hidden property MainStartTime

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `val` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `StopTime()`

### Syntax
```matlab
function val = StopTime(obj)
```
Defined at source line `206`.

### Description
STOPTIME Return the end time of the measurement. val = obj.StopTime() or val = StopTime(obj) Returns the time passed from the creation of the object to stopping of the object. The stop time is stored in the hidden property MainStopTime

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `val` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `par2struct()`

### Syntax
```matlab
function parInfo = par2struct(obj)
```
Defined at source line `218`.

### Description
PAR2STRUCT Convert the results to a flat structure. p = obj.par2struct() or p = par2struct(obj) Converts the results into a flat structure with the following fields: Start : start times of each PARFOR block Stop : end times of each PARFOR block Worker : array of process id's for each iteration ItStart : array of start times for each iteration ItStop : array of stop times for each iteration

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `parInfo` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Tips
Handles NaN, Inf, or finite-value filtering.

### Algorithms
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** Parallel Computing Toolbox
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `plot()`

### Syntax
```matlab
function plot(obj, varargin)
```
Defined at source line `238`.

### Description
PLOT Create a custom plot of the results. obj.plot() or plot(obj) Creates a custom plot of the results. The plot consists of 3 parts: 1) a line graph showing start and stop times of each iteration on each worker. 2) a stacked bar graph showing the efficiency of each worker. 3) a plot showing actual duration of each iteration. obj.plot(obj2) or plot(obj, obj2) Creates a custom plot that also compares the results of obj and obj2. obj2 must be of class Par and must be a result from a serial computation or a single-worker computation. Error checking

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
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
Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

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

## `tic()`

### Syntax
```matlab
function val = tic()
```
Defined at source line `318`.

### Description
TIC Record start time of parfor loop iteration. Par.tic() Records the starting time within the loop. This should be called immediately inside the parfor loop. See also Par.toc

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `val` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** Parallel Computing Toolbox
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `toc()`

### Syntax
```matlab
function obj = toc()
```
Defined at source line `341`.

### Description
TOC Record stop time of parfor loop iteration. obj = Par.toc() Records the ending time within the loop. This should be called just before the end statement of the parfor loop. See also Par.tic

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `obj` — MATLAB App/UI object or callback handle
Output produced by the MATLAB implementation.

### More About
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** Parallel Computing Toolbox
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `vertcat()`

### Syntax
```matlab
function varargout = vertcat(varargin) %#ok<STOUT>
```
Defined at source line `370`.

### Description
Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `varargout` — cell array of variable MATLAB arguments
Output produced by the MATLAB implementation.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `addlistener()`

### Syntax
```matlab
function out = addlistener(varargin)
```
Defined at source line `378`.

### Description
Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `out` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

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
function delete(varargin)
```
Defined at source line `382`.

### Description
Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `eq()`

### Syntax
```matlab
function out = eq(varargin)
```
Defined at source line `386`.

### Description
Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `out` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `findobj()`

### Syntax
```matlab
function findobj(varargin)
```
Defined at source line `390`.

### Description
Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** `BrainNetViewer_20191031/BrainNet.m:363/NV_m_exit_Callback`, `BrainNetViewer_20191031/BrainNet_EdgCostumColor.m:147/pushbutton1_Callback`, `BrainNetViewer_20191031/BrainNet_EdgCostumColor.m:157/pushbutton2_Callback`, `BrainNetViewer_20191031/BrainNet_LoadFiles.m:104/OK_button_Callback`, `BrainNetViewer_20191031/BrainNet_LoadFiles.m:62/BrainNet_LoadFiles_OpeningFcn`, `BrainNetViewer_20191031/BrainNet_LoadFiles.m:809/Cancel_button_Callback`, `BrainNetViewer_20191031/BrainNet_MergeMesh.m:504/Cancel_button_Callback`, `BrainNetViewer_20191031/BrainNet_MergeMesh.m:60/BrainNet_MergeMesh_OpeningFcn`, `BrainNetViewer_20191031/BrainNet_ModuleColor.m:147/pushbutton1_Callback`, `BrainNetViewer_20191031/BrainNet_ModuleColor.m:157/pushbutton2_Callback`, `BrainNetViewer_20191031/BrainNet_Option.m:1188/OK_button_Callback`, `BrainNetViewer_20191031/BrainNet_Option.m:1533/Cancel_button_Callback`, `BrainNetViewer_20191031/vrml.m:111/HandleAxes`, `whifun_functions/whifun_paint.m:1/whifun_paint`, `whifun_qcviewer.mlapp:358/themeChildren`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `BrainNetViewer_20191031/BrainNet.m:363/NV_m_exit_Callback`, `BrainNetViewer_20191031/BrainNet_EdgCostumColor.m:147/pushbutton1_Callback`, `BrainNetViewer_20191031/BrainNet_EdgCostumColor.m:157/pushbutton2_Callback`, `BrainNetViewer_20191031/BrainNet_LoadFiles.m:104/OK_button_Callback`, `BrainNetViewer_20191031/BrainNet_LoadFiles.m:62/BrainNet_LoadFiles_OpeningFcn`, `BrainNetViewer_20191031/BrainNet_LoadFiles.m:809/Cancel_button_Callback`, `BrainNetViewer_20191031/BrainNet_MergeMesh.m:504/Cancel_button_Callback`, `BrainNetViewer_20191031/BrainNet_MergeMesh.m:60/BrainNet_MergeMesh_OpeningFcn`, `BrainNetViewer_20191031/BrainNet_ModuleColor.m:147/pushbutton1_Callback`, `BrainNetViewer_20191031/BrainNet_ModuleColor.m:157/pushbutton2_Callback`, `BrainNetViewer_20191031/BrainNet_Option.m:1188/OK_button_Callback`, `BrainNetViewer_20191031/BrainNet_Option.m:1533/Cancel_button_Callback`, `BrainNetViewer_20191031/vrml.m:111/HandleAxes`, `whifun_functions/whifun_paint.m:1/whifun_paint`, `whifun_qcviewer.mlapp:358/themeChildren`

## `findprop()`

### Syntax
```matlab
function out = findprop(varargin)
```
Defined at source line `394`.

### Description
Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `out` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `ge()`

### Syntax
```matlab
function out = ge(varargin)
```
Defined at source line `398`.

### Description
Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `out` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `gt()`

### Syntax
```matlab
function out = gt(varargin)
```
Defined at source line `402`.

### Description
Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `out` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `le()`

### Syntax
```matlab
function out = le(varargin)
```
Defined at source line `406`.

### Description
Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `out` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `lt()`

### Syntax
```matlab
function out = lt(varargin)
```
Defined at source line `410`.

### Description
Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `out` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `ne()`

### Syntax
```matlab
function out = ne(varargin)
```
Defined at source line `414`.

### Description
Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `out` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `notify()`

### Syntax
```matlab
function notify(varargin)
```
Defined at source line `418`.

### Description
Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `getnow()`

### Syntax
```matlab
function out = getnow(flag)
```
Defined at source line `426`.

### Description
getnow Internal function for recording global start time (in serial dates).

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `flag` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `out` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Tips
Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `tictoc()`

### Syntax
```matlab
function out = tictoc(flag)
```
Defined at source line `447`.

### Description
tictoc Internal function for recording start and end times.

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `flag` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `out` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Tips
Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `parPlot()`

### Syntax
```matlab
function  parPlot(addSerial, parInfo, varargin)
```
Defined at source line `476`.

### Description
Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `addSerial` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `parInfo` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `setScaleFcn()`

### Syntax
```matlab
function setScaleFcn(hObject, ~, hAx)
```
Defined at source line `673`.

### Description
Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `hObject` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `~` — unused placeholder
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `hAx` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

# Module Name: `parTicToc/Par.m`
- **Module Category:** Bundled parallel timing helper.
- **Theoretical Background:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: Parallel Computing Toolbox

## Function: `Par()`
- **Signature & Definition:** `classdef Par < handle` (line 1)
- **Scientific Theory & Formulas:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR measurements StartTime - Return the start time of the measurement StopTime - Return the stop time of 
- **Arguments:**
  - No explicit input arguments.
- **Returns:**
  - `Par` (MATLAB App or class type): Class definition used to instantiate the module.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: Parallel Computing Toolbox
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `Par()`
- **Signature & Definition:** `function obj = Par(n, varargin)` (line 81)
- **Scientific Theory & Formulas:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Functional Purpose:** PAR Contructor for the Par object obj = Par(N) Creates an array of loop timer object for PARFOR loops. N is a positive integer equal to the length of iterations in the PARFOR loop. Special case used internally check first since we want this to happen immediately.
- **Arguments:**
  - `n` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `obj` (MATLAB App/UI object or callback handle): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: Parallel Computing Toolbox
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

## Function: `horzcat()`
- **Signature & Definition:** `function newobj = horzcat(varargin)` (line 122)
- **Scientific Theory & Formulas:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Functional Purpose:** HORZCAT Horizontally concatenate multiple PARFOR measurements. horzcat(p1, p2, ...) or [p1, p2, ...] Concatenates multiple Par objects. This allows you to combine results from multiple PARFOR blocks that are run sequentially. P1, P2, ... must be either Par objects or an empty array ([]).
- **Arguments:**
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `newobj` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: Parallel Computing Toolbox
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

## Function: `stop()`
- **Signature & Definition:** `function stop(obj)` (line 171)
- **Scientific Theory & Formulas:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Functional Purpose:** STOP Stop the measurement. obj.stop() or stop(obj) Stops the measurement process. This should be called right after the parfor loop.
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: Parallel Computing Toolbox
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

## Function: `StartTime()`
- **Signature & Definition:** `function val = StartTime(obj)` (line 189)
- **Scientific Theory & Formulas:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Functional Purpose:** STARTTIME Return the end time of the measurement. val = obj.StartTime() or val = StartTime(obj) Returns the start time relative to the initial creation of the object. Usually, this is zero. If this object was a concatenation of multiple Par objects, then this will return multiple start times for each of the objects, relative to the initial start time. The start time is stored in the hidden property MainStartTime
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `val` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `StopTime()`
- **Signature & Definition:** `function val = StopTime(obj)` (line 206)
- **Scientific Theory & Formulas:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Functional Purpose:** STOPTIME Return the end time of the measurement. val = obj.StopTime() or val = StopTime(obj) Returns the time passed from the creation of the object to stopping of the object. The stop time is stored in the hidden property MainStopTime
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `val` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `par2struct()`
- **Signature & Definition:** `function parInfo = par2struct(obj)` (line 218)
- **Scientific Theory & Formulas:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Functional Purpose:** PAR2STRUCT Convert the results to a flat structure. p = obj.par2struct() or p = par2struct(obj) Converts the results into a flat structure with the following fields: Start : start times of each PARFOR block Stop : end times of each PARFOR block Worker : array of process id's for each iteration ItStart : array of start times for each iteration ItStop : array of stop times for each iteration
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `parInfo` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: Parallel Computing Toolbox
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Handles NaN, Inf, or finite-value filtering.

## Function: `plot()`
- **Signature & Definition:** `function plot(obj, varargin)` (line 238)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** PLOT Create a custom plot of the results. obj.plot() or plot(obj) Creates a custom plot of the results. The plot consists of 3 parts: 1) a line graph showing start and stop times of each iteration on each worker. 2) a stacked bar graph showing the efficiency of each worker. 3) a plot showing actual duration of each iteration. obj.plot(obj2) or plot(obj, obj2) Creates a custom plot that also compares the results of obj and obj2. obj2 must be of class Par and must be a result from a serial computation or a single-worker computation. Error checking
- **Arguments:**
  - `obj` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

## Function: `tic()`
- **Signature & Definition:** `function val = tic()` (line 318)
- **Scientific Theory & Formulas:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Functional Purpose:** TIC Record start time of parfor loop iteration. Par.tic() Records the starting time within the loop. This should be called immediately inside the parfor loop. See also Par.toc
- **Arguments:**
  - No explicit input arguments.
- **Returns:**
  - `val` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: Parallel Computing Toolbox
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections.

## Function: `toc()`
- **Signature & Definition:** `function obj = toc()` (line 341)
- **Scientific Theory & Formulas:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Functional Purpose:** TOC Record stop time of parfor loop iteration. obj = Par.toc() Records the ending time within the loop. This should be called just before the end statement of the parfor loop. See also Par.tic
- **Arguments:**
  - No explicit input arguments.
- **Returns:**
  - `obj` (MATLAB App/UI object or callback handle): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: Parallel Computing Toolbox
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections.

## Function: `vertcat()`
- **Signature & Definition:** `function varargout = vertcat(varargin) %#ok<STOUT>` (line 370)
- **Scientific Theory & Formulas:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m
- **Arguments:**
  - No explicit input arguments.
- **Returns:**
  - `varargout` (cell array of variable MATLAB arguments): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

## Function: `addlistener()`
- **Signature & Definition:** `function out = addlistener(varargin)` (line 378)
- **Scientific Theory & Formulas:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m
- **Arguments:**
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `out` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `delete()`
- **Signature & Definition:** `function delete(varargin)` (line 382)
- **Scientific Theory & Formulas:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. App Designer methods coordinate user interaction and inherit mathematical content from called WhiFuN routines.
- **Functional Purpose:** Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m
- **Arguments:**
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `eq()`
- **Signature & Definition:** `function out = eq(varargin)` (line 386)
- **Scientific Theory & Formulas:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m
- **Arguments:**
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `out` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `findobj()`
- **Signature & Definition:** `function findobj(varargin)` (line 390)
- **Scientific Theory & Formulas:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m
- **Arguments:**
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: `BrainNetViewer_20191031/BrainNet.m:363/NV_m_exit_Callback`, `BrainNetViewer_20191031/BrainNet_EdgCostumColor.m:147/pushbutton1_Callback`, `BrainNetViewer_20191031/BrainNet_EdgCostumColor.m:157/pushbutton2_Callback`, `BrainNetViewer_20191031/BrainNet_LoadFiles.m:104/OK_button_Callback`, `BrainNetViewer_20191031/BrainNet_LoadFiles.m:62/BrainNet_LoadFiles_OpeningFcn`, `BrainNetViewer_20191031/BrainNet_LoadFiles.m:809/Cancel_button_Callback`, `BrainNetViewer_20191031/BrainNet_MergeMesh.m:504/Cancel_button_Callback`, `BrainNetViewer_20191031/BrainNet_MergeMesh.m:60/BrainNet_MergeMesh_OpeningFcn`, `BrainNetViewer_20191031/BrainNet_ModuleColor.m:147/pushbutton1_Callback`, `BrainNetViewer_20191031/BrainNet_ModuleColor.m:157/pushbutton2_Callback`, `BrainNetViewer_20191031/BrainNet_Option.m:1188/OK_button_Callback`, `BrainNetViewer_20191031/BrainNet_Option.m:1533/Cancel_button_Callback`, `BrainNetViewer_20191031/vrml.m:111/HandleAxes`, `whifun_functions/whifun_paint.m:1/whifun_paint`, `whifun_qcviewer.mlapp:358/themeChildren`
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `findprop()`
- **Signature & Definition:** `function out = findprop(varargin)` (line 394)
- **Scientific Theory & Formulas:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m
- **Arguments:**
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `out` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `ge()`
- **Signature & Definition:** `function out = ge(varargin)` (line 398)
- **Scientific Theory & Formulas:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m
- **Arguments:**
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `out` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `gt()`
- **Signature & Definition:** `function out = gt(varargin)` (line 402)
- **Scientific Theory & Formulas:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m
- **Arguments:**
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `out` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `le()`
- **Signature & Definition:** `function out = le(varargin)` (line 406)
- **Scientific Theory & Formulas:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m
- **Arguments:**
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `out` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `lt()`
- **Signature & Definition:** `function out = lt(varargin)` (line 410)
- **Scientific Theory & Formulas:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m
- **Arguments:**
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `out` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `ne()`
- **Signature & Definition:** `function out = ne(varargin)` (line 414)
- **Scientific Theory & Formulas:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m
- **Arguments:**
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `out` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `notify()`
- **Signature & Definition:** `function notify(varargin)` (line 418)
- **Scientific Theory & Formulas:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m
- **Arguments:**
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `getnow()`
- **Signature & Definition:** `function out = getnow(flag)` (line 426)
- **Scientific Theory & Formulas:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Functional Purpose:** getnow Internal function for recording global start time (in serial dates).
- **Arguments:**
  - `flag` (logical or numeric flag): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `out` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

## Function: `tictoc()`
- **Signature & Definition:** `function out = tictoc(flag)` (line 447)
- **Scientific Theory & Formulas:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Functional Purpose:** tictoc Internal function for recording start and end times.
- **Arguments:**
  - `flag` (logical or numeric flag): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `out` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

## Function: `parPlot()`
- **Signature & Definition:** `function  parPlot(addSerial, parInfo, varargin)` (line 476)
- **Scientific Theory & Formulas:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m
- **Arguments:**
  - `addSerial` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `parInfo` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering.

## Function: `setScaleFcn()`
- **Signature & Definition:** `function setScaleFcn(hObject, ~, hAx)` (line 673)
- **Scientific Theory & Formulas:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** Par TIC-TOC class for parfor loops This is a class for timing PARFOR loops. Once the measurement is made, it can be plotted to observe the various overheads that may exist in parallel for loops. It also shows the utilization of each worker. Par Properties: Worker - Process ID of the worker ItStart - Start time of iteration ItStop - Stop time of iteration Par Methods: Par - Construct Par objects and start the measurement stop - Stop the measurement par2struct - Convert the results to a flat structure plot - Create a custom plot of the results horzcat - Horizontally concatenate multiple PARFOR m
- **Arguments:**
  - `hObject` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `~` (unused placeholder): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `hAx` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

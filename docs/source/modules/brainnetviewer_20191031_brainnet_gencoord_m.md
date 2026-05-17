# Module Name: `BrainNetViewer_20191031/BrainNet_GenCoord.m`
- **Module Category:** Bundled BrainNetViewer dependency.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia Function to generate node file from voxel-based template ----------------------------------------------------------- Copyright(c) 2015 State Key Laboratory of Cognitive Neuroscience and Learning, Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.52; Date 20150306; Last edited 20150306 ----------------------------------------------------------- Usage: BrainNet_GenCoord(filename,outputfilename); filenames is the name of the voxel-based template file. o
  - Internal calls detected: `coord`
  - External dependencies detected: SPM12, BrainNet Viewer

## Function: `BrainNet_GenCoord()`
- **Signature & Definition:** `function BrainNet_GenCoord(filename,outputfilename, regions)` (line 1)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia Function to generate node file from voxel-based template ----------------------------------------------------------- Copyright(c) 2015 State Key Laboratory of Cognitive Neuroscience and Learning, Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.52; Date 20150306; Last edited 20150306 ----------------------------------------------------------- Usage: BrainNet_GenCoord(filename,outputfilename); filenames is the name of the voxel-based template file. outputfilename is the name of the output node file. regions is the wanted index in the template. Exam
- **Arguments:**
  - `filename` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `outputfilename` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `regions` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: `coord`
  - External: SPM12, BrainNet Viewer
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files.

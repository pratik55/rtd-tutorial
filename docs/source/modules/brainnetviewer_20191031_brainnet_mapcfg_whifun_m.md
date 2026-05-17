# Module Name: `BrainNetViewer_20191031/BrainNet_MapCfg_WhifuN.m`
- **Module Category:** Bundled BrainNetViewer dependency.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia Function to draw graph from commandline ----------------------------------------------------------- Copyright(c) 2013 State Key Laboratory of Cognitive Neuroscience and Learning, Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.52; Date 20121031; Last edited 20150414 ----------------------------------------------------------- Usage: H_BrainNet = BrainNet_MapCfg(Filenames); Filenames can be any kinds of files supported by BrainNet Viewer. Example: Su
  - Internal calls detected: `BrainNet`
  - External dependencies detected: MATLAB NIfTI I/O, MATLAB table/file I/O, SPM12, BrainNet Viewer

## Function: `BrainNet_MapCfg_WhifuN()`
- **Signature & Definition:** `function H_BrainNet = BrainNet_MapCfg_WhifuN(varargin)` (line 1)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** BrainNet Viewer, a graph-based brain network mapping tool, by Mingrui Xia Function to draw graph from commandline ----------------------------------------------------------- Copyright(c) 2013 State Key Laboratory of Cognitive Neuroscience and Learning, Beijing Normal University Written by Mingrui Xia Mail to Author: <a href="mingruixia@gmail.com">Mingrui Xia</a> Version 1.52; Date 20121031; Last edited 20150414 ----------------------------------------------------------- Usage: H_BrainNet = BrainNet_MapCfg(Filenames); Filenames can be any kinds of files supported by BrainNet Viewer. Example: Surface file only: BrainNet_MapCfg('BrainMesh_ICBM152.nv'); Surface and node files: BrainNet_MapCfg('B
- **Arguments:**
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `H_BrainNet` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `BrainNet`
  - External: MATLAB NIfTI I/O, MATLAB table/file I/O, SPM12, BrainNet Viewer
  - Called By: `main.mlapp:1145/DisplayFNButtonPushed`, `whifun_functions/whifun_create_brainnet_images.m:1/whifun_create_brainnet_images`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections.

# Module Name: `whifun.m`
- **Module Category:** Top-level WhiFuN entry point.
- **Theoretical Background:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Key Features:**
  - WHIFUN White matter Functional Networks (WhiFuN) Toolbox Main Function. WHIFUN is the primary entry point for the GUI-based WhiFuN Toolbox, a comprehensive suite of tools for investigating brain functional connectivity in White Matter (WM) and Gray Matter (GM). It fully automates preprocessing steps to derive BOLD signals for WM and GM analysis. To start the GUI: >> whifun Requires: - MATLAB R2022a or later (recommended). - Image Processing Toolbox - Signal Processing Toolbox - Statistics and Machine Learning Toolbox - Bioinformatics Toolbox - SPM12 toolbox (must be downloaded and added to MAT
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: BrainNet Viewer

## Function: `whifun()`
- **Signature & Definition:** `function whifun(varargin)` (line 1)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN White matter Functional Networks (WhiFuN) Toolbox Main Function. WHIFUN is the primary entry point for the GUI-based WhiFuN Toolbox, a comprehensive suite of tools for investigating brain functional connectivity in White Matter (WM) and Gray Matter (GM). It fully automates preprocessing steps to derive BOLD signals for WM and GM analysis. To start the GUI: >> whifun Requires: - MATLAB R2022a or later (recommended). - Image Processing Toolbox - Signal Processing Toolbox - Statistics and Machine Learning Toolbox - Bioinformatics Toolbox - SPM12 toolbox (must be downloaded and added to MATLAB path). The function initializes the environment, displays a welcome message, provides links to d
- **Arguments:**
  - `varargin` (cell array of variable MATLAB arguments): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: BrainNet Viewer
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files.

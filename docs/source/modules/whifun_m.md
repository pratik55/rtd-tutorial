# Module Name: `whifun.m`

## Description
- **Module Category:** Top-level WhiFuN entry point.
- **Theoretical Background:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Key Features:**
  - WHIFUN White matter Functional Networks (WhiFuN) Toolbox Main Function. WHIFUN is the primary entry point for the GUI-based WhiFuN Toolbox, a comprehensive suite of tools for investigating brain functional connectivity in White Matter (WM) and Gray Matter (GM). It fully automates preprocessing steps to derive BOLD signals for WM and GM analysis. To start the GUI: >> whifun Requires: - MATLAB R2022a or later (recommended). - Image Processing Toolbox - Signal Processing Toolbox - Statistics and Machine Learning Toolbox - Bioinformatics Toolbox - SPM12 toolbox (must be downloaded and added to MAT
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: BrainNet Viewer

## `whifun()`

### Syntax
```matlab
function whifun(varargin)
```
Defined at source line `1`.

### Description
WHIFUN White matter Functional Networks (WhiFuN) Toolbox Main Function. WHIFUN is the primary entry point for the GUI-based WhiFuN Toolbox, a comprehensive suite of tools for investigating brain functional connectivity in White Matter (WM) and Gray Matter (GM). It fully automates preprocessing steps to derive BOLD signals for WM and GM analysis. To start the GUI: >> whifun Requires: - MATLAB R2022a or later (recommended). - Image Processing Toolbox - Signal Processing Toolbox - Statistics and Machine Learning Toolbox - Bioinformatics Toolbox - SPM12 toolbox (must be downloaded and added to MATLAB path). The function initializes the environment, displays a welcome message, provides links to d

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

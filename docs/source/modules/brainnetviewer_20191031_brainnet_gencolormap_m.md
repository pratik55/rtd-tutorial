# Module Name: `BrainNetViewer_20191031/BrainNet_GenColormap.m`
- **Module Category:** Bundled BrainNetViewer dependency.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - No leading help block was present; behavior was inferred from signatures and static calls.
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: BrainNet Viewer

## Function: `BrainNet_GenColormap()`
- **Signature & Definition:** `function c = BrainNet_GenColormap(Nmax,Nmin,Pmin,Pmax,original_color_map)` (line 1)
- **Scientific Theory & Formulas:** Normalized mutual information is $NMI=\frac{2I(X;Y)}{H(X)+H(Y)}$, where $I(X;Y)=\sum_{ij}p_{ij}\log_2\frac{p_{ij}}{p_i p_j}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** Routine has no dedicated help block; purpose was inferred from its name, surrounding module, and static call context.
- **Arguments:**
  - `Nmax` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `Nmin` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `Pmin` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `Pmax` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `original_color_map` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `c` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: BrainNet Viewer
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections.

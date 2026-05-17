# Module Name: `BrainNetViewer_20191031/BrainNet_GenColormap.m`

## Description
- **Module Category:** Bundled BrainNetViewer dependency.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - No leading help block was present; behavior was inferred from signatures and static calls.
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: BrainNet Viewer

## `BrainNet_GenColormap()`

### Syntax
```matlab
function c = BrainNet_GenColormap(Nmax,Nmin,Pmin,Pmax,original_color_map)
```
Defined at source line `1`.

### Description
Routine has no dedicated help block; purpose was inferred from its name, surrounding module, and static call context.

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `Nmax` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Nmin` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Pmin` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Pmax` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `original_color_map` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `c` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Normalized mutual information is $NMI=\frac{2I(X;Y)}{H(X)+H(Y)}$, where $I(X;Y)=\sum_{ij}p_{ij}\log_2\frac{p_{ij}}{p_i p_j}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
Normalized mutual information is $NMI=\frac{2I(X;Y)}{H(X)+H(Y)}$, where $I(X;Y)=\sum_{ij}p_{ij}\log_2\frac{p_{ij}}{p_i p_j}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** BrainNet Viewer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

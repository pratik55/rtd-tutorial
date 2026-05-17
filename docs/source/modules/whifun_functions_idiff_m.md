# Module Name: `whifun_functions/idiff.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Identifiability uses $I_{diff}=100(\overline{|r_{self}|}-\overline{|r_{other}|})$ and nearest-neighbor FC matching accuracy. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - % Input vec1 -> FC of all subjects first session vec2 -> FC of all subjects second session fig_op -> 1 -> plots the A matrix fig_op -> 0 -> does not plot the matrix pca_op -> 1 -> do pca pca _op -> 0 -> no pca
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: Statistics and Machine Learning Toolbox

## `idiff()`

### Syntax
```matlab
function [idiff_score,A,Iself,Iothers] = idiff(vec1,vec2,fig_op,pca_op)
```
Defined at source line `1`.

### Description
% Input vec1 -> FC of all subjects first session vec2 -> FC of all subjects second session fig_op -> 1 -> plots the A matrix fig_op -> 0 -> does not plot the matrix pca_op -> 1 -> do pca pca _op -> 0 -> no pca

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `vec1` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `vec2` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `fig_op` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `pca_op` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `idiff_score` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `A` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `Iself` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `Iothers` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Identifiability uses $I_{diff}=100(\overline{|r_{self}|}-\overline{|r_{other}|})$ and nearest-neighbor FC matching accuracy. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
Defines defaults or branches for optional arguments or missing files.

### Algorithms
Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Identifiability uses $I_{diff}=100(\overline{|r_{self}|}-\overline{|r_{other}|})$ and nearest-neighbor FC matching accuracy. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** Statistics and Machine Learning Toolbox
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

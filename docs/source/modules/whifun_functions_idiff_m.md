# Module Name: `whifun_functions/idiff.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Identifiability uses $I_{diff}=100(\overline{|r_{self}|}-\overline{|r_{other}|})$ and nearest-neighbor FC matching accuracy. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - % Input vec1 -> FC of all subjects first session vec2 -> FC of all subjects second session fig_op -> 1 -> plots the A matrix fig_op -> 0 -> does not plot the matrix pca_op -> 1 -> do pca pca _op -> 0 -> no pca
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: Statistics and Machine Learning Toolbox

## Function: `idiff()`
- **Signature & Definition:** `function [idiff_score,A,Iself,Iothers] = idiff(vec1,vec2,fig_op,pca_op)` (line 1)
- **Scientific Theory & Formulas:** Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Identifiability uses $I_{diff}=100(\overline{|r_{self}|}-\overline{|r_{other}|})$ and nearest-neighbor FC matching accuracy. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** % Input vec1 -> FC of all subjects first session vec2 -> FC of all subjects second session fig_op -> 1 -> plots the A matrix fig_op -> 0 -> does not plot the matrix pca_op -> 1 -> do pca pca _op -> 0 -> no pca
- **Arguments:**
  - `vec1` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `vec2` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `fig_op` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `pca_op` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `idiff_score` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
  - `A` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
  - `Iself` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
  - `Iothers` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: Statistics and Machine Learning Toolbox
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files.

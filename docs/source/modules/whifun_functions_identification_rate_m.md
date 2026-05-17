# Module Name: `whifun_functions/identification_rate.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Identifiability uses $I_{diff}=100(\overline{|r_{self}|}-\overline{|r_{other}|})$ and nearest-neighbor FC matching accuracy.
- **Key Features:**
  - % Inputs vec1 = FC vector for 1st session of all subjects vec2 = FC vector for 2nd session of all subjects
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: Statistics and Machine Learning Toolbox

## `identification_rate()`

### Syntax
```matlab
function [acco,confu_] = identification_rate(vec1,vec2)
```
Defined at source line `1`.

### Description
% Inputs vec1 = FC vector for 1st session of all subjects vec2 = FC vector for 2nd session of all subjects

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `vec1` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `vec2` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `acco` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `confu_` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Identifiability uses $I_{diff}=100(\overline{|r_{self}|}-\overline{|r_{other}|})$ and nearest-neighbor FC matching accuracy.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Identifiability uses $I_{diff}=100(\overline{|r_{self}|}-\overline{|r_{other}|})$ and nearest-neighbor FC matching accuracy.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** Statistics and Machine Learning Toolbox
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

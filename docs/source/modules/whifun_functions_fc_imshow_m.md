# Module Name: `whifun_functions/fc_imshow.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - FC_IMSHOW Displays a functional connectivity (FC) matrix with network boundaries and labels. FC_IMSHOW(MAP, SORT_IDX_VAL, NET_NAMES) This function visualizes a functional connectivity matrix, typically one that has been reordered based on network assignments, and overlays black lines to demarcate the boundaries between the identified networks. It also labels the axes with the network names or indices. Input Arguments: MAP - The functional connectivity matrix (N x N) to display. Should be symmetric and ideally sorted by network assignment. SORT_IDX_VAL - A vector (N x 1) containing the network
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `fc_imshow()`

### Syntax
```matlab
function fc_imshow(map,sort_idx_val,net_names)
```
Defined at source line `1`.

### Description
FC_IMSHOW Displays a functional connectivity (FC) matrix with network boundaries and labels. FC_IMSHOW(MAP, SORT_IDX_VAL, NET_NAMES) This function visualizes a functional connectivity matrix, typically one that has been reordered based on network assignments, and overlays black lines to demarcate the boundaries between the identified networks. It also labels the axes with the network names or indices. Input Arguments: MAP - The functional connectivity matrix (N x N) to display. Should be symmetric and ideally sorted by network assignment. SORT_IDX_VAL - A vector (N x 1) containing the network index for each ROI/voxel in the MAP matrix. The map is assumed to be sorted such that all elements b

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `map` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `sort_idx_val` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `net_names` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
Defines defaults or branches for optional arguments or missing files.

### Algorithms
Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

# Module Name: `whifun_functions/private/pr_scaletocmap.m`

## Description
- **Module Category:** Private visualization/helper dependency.
- **Theoretical Background:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$.
- **Key Features:**
  - Scale image data to colormap, returning colormap indices FORMAT [img, badvals]=pr_scaletocmap(inpimg,mn,mx,cmap,lrn) Inputs inpimg - matrix containing image to scale mn - image value that maps to first value of colormap mx - image value that maps to last value of colormap cmap - 3xN colormap lrn - 1x3 vector, giving colormap indices that should fill: - lrn(1) (L=Left) - values less than mn - lrn(2) (R=Right) - values greater than mx - lrn(3) (N=NaN) - NaN values If lrn value is 0, then colormap values are set to 1, and indices to these values are returned in badvals (below) Output img - inpimg
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `pr_scaletocmap()`

### Syntax
```matlab
function [img, badvals]=pr_scaletocmap(inpimg,mn,mx,cmap,lrn)
```
Defined at source line `1`.

### Description
Scale image data to colormap, returning colormap indices FORMAT [img, badvals]=pr_scaletocmap(inpimg,mn,mx,cmap,lrn) Inputs inpimg - matrix containing image to scale mn - image value that maps to first value of colormap mx - image value that maps to last value of colormap cmap - 3xN colormap lrn - 1x3 vector, giving colormap indices that should fill: - lrn(1) (L=Left) - values less than mn - lrn(2) (R=Right) - values greater than mx - lrn(3) (N=NaN) - NaN values If lrn value is 0, then colormap values are set to 1, and indices to these values are returned in badvals (below) Output img - inpimg scaled between 1 and (size(cmap, 1)) badvals - indices into inpimg containing values out of range,

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `inpimg` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `mn` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `mx` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `cmap` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `lrn` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `img` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `badvals` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$.

### Tips
Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** `whifun_functions/whifun_paint.m:1/whifun_paint`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `whifun_functions/whifun_paint.m:1/whifun_paint`

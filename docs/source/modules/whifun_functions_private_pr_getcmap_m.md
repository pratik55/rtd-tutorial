# Module Name: `whifun_functions/private/pr_getcmap.m`

## Description
- **Module Category:** Private visualization/helper dependency.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - Get colormap of name acmapname FORMAT [cmap, warnstr] = pr_getcmap(acmapname) Inputs acmapname - string. Can be (in order of precedence) - matrix name in base workspace - colour name; one of 'red','green','blue','cyan', 'magenta', 'yellow', 'black', 'white' - filename of .mat or .lut file. If filename has no extension, assumes '.mat' extension Outputs cmap - Nx3 colormap matrix or empty if fails warnstr - warning message if fails __________________________________________________________________________ Matthew Brett $Id: pr_getcmap.m 6623 2015-12-03 18:38:08Z guillaume $
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: MATLAB table/file I/O, SLover/MarsBaR-style visualization helpers

## `pr_getcmap()`

### Syntax
```matlab
function [cmap, warnstr] = pr_getcmap(acmapname)
```
Defined at source line `1`.

### Description
Get colormap of name acmapname FORMAT [cmap, warnstr] = pr_getcmap(acmapname) Inputs acmapname - string. Can be (in order of precedence) - matrix name in base workspace - colour name; one of 'red','green','blue','cyan', 'magenta', 'yellow', 'black', 'white' - filename of .mat or .lut file. If filename has no extension, assumes '.mat' extension Outputs cmap - Nx3 colormap matrix or empty if fails warnstr - warning message if fails __________________________________________________________________________ Matthew Brett $Id: pr_getcmap.m 6623 2015-12-03 18:38:08Z guillaume $

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `acmapname` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `cmap` — numeric scalar, vector, matrix, or multidimensional array
Output produced by the MATLAB implementation.

#### `warnstr` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** MATLAB table/file I/O, SLover/MarsBaR-style visualization helpers
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

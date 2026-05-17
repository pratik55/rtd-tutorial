# Module Name: `whifun_functions/private/pr_getcmap.m`
- **Module Category:** Private visualization/helper dependency.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - Get colormap of name acmapname FORMAT [cmap, warnstr] = pr_getcmap(acmapname) Inputs acmapname - string. Can be (in order of precedence) - matrix name in base workspace - colour name; one of 'red','green','blue','cyan', 'magenta', 'yellow', 'black', 'white' - filename of .mat or .lut file. If filename has no extension, assumes '.mat' extension Outputs cmap - Nx3 colormap matrix or empty if fails warnstr - warning message if fails __________________________________________________________________________ Matthew Brett $Id: pr_getcmap.m 6623 2015-12-03 18:38:08Z guillaume $
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: MATLAB table/file I/O, SLover/MarsBaR-style visualization helpers

## Function: `pr_getcmap()`
- **Signature & Definition:** `function [cmap, warnstr] = pr_getcmap(acmapname)` (line 1)
- **Scientific Theory & Formulas:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** Get colormap of name acmapname FORMAT [cmap, warnstr] = pr_getcmap(acmapname) Inputs acmapname - string. Can be (in order of precedence) - matrix name in base workspace - colour name; one of 'red','green','blue','cyan', 'magenta', 'yellow', 'black', 'white' - filename of .mat or .lut file. If filename has no extension, assumes '.mat' extension Outputs cmap - Nx3 colormap matrix or empty if fails warnstr - warning message if fails __________________________________________________________________________ Matthew Brett $Id: pr_getcmap.m 6623 2015-12-03 18:38:08Z guillaume $
- **Arguments:**
  - `acmapname` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `cmap` (numeric scalar, vector, matrix, or multidimensional array): Output produced by the MATLAB implementation.
  - `warnstr` (numeric scalar or numeric vector): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: MATLAB table/file I/O, SLover/MarsBaR-style visualization helpers
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions.

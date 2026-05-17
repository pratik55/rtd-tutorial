# Module Name: `parTicToc/sweepExample.m`
- **Module Category:** Bundled parallel timing helper.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - Copyright 2010 The MathWorks, Inc. % Initialize Problem
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: Parallel Computing Toolbox

## Function: `sweepExample()`
- **Signature & Definition:** `function parInfo = sweepExample()` (line 1)
- **Scientific Theory & Formulas:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** Copyright 2010 The MathWorks, Inc. % Initialize Problem
- **Arguments:**
  - No explicit input arguments.
- **Returns:**
  - `parInfo` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: Parallel Computing Toolbox
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Handles NaN, Inf, or finite-value filtering. Depends on external command availability and shell exit status.

## Function: `odesystem()`
- **Signature & Definition:** `function dy = odesystem(t, y, m, b, k)` (line 31)
- **Scientific Theory & Formulas:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Functional Purpose:** 2nd-order ODE m*X'' + b*X' + k*X = 0 --> system of 1st-order ODEs y = X' y' = -1/m * (k*y + b*y')
- **Arguments:**
  - `t` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `y` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `m` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `b` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `k` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `dy` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Depends on external command availability and shell exit status.

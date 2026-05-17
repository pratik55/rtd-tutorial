# Module Name: `whifun_functions/private/mars_struct.m`

## Description
- **Module Category:** Private visualization/helper dependency.
- **Theoretical Background:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Key Features:**
  - Multifunction function for manipulating structures To help the exposition a bit: 'fill' in a name, means that values empty or missing in one structure are fetched from another 'merge' means simply that missing fields are added, with values, from a second structure (but not filled if empty) Each function needs to deal with the case of empty arguments FORMAT c = mars_struct('fillafromb', a, b, fieldns, flags) fills structure fields empty or missing in a from those present in b a, b are structures fieldns (optional) is cell array of field names to fill from in b c is returned structure Is recursi
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: SLover/MarsBaR-style visualization helpers

## `mars_struct()`

### Syntax
```matlab
function varargout = mars_struct(action, varargin)
```
Defined at source line `1`.

### Description
Multifunction function for manipulating structures To help the exposition a bit: 'fill' in a name, means that values empty or missing in one structure are fetched from another 'merge' means simply that missing fields are added, with values, from a second structure (but not filled if empty) Each function needs to deal with the case of empty arguments FORMAT c = mars_struct('fillafromb', a, b, fieldns, flags) fills structure fields empty or missing in a from those present in b a, b are structures fieldns (optional) is cell array of field names to fill from in b c is returned structure Is recursive, will fill struct fields from struct fields flags may contain 'f', which Force fills a from b (al

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `action` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `varargout` — cell array of variable MATLAB arguments
Output produced by the MATLAB implementation.

### More About
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Tips
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** SLover/MarsBaR-style visualization helpers
- **Called By:** `whifun_functions/private/pr_volmaxmin.m:1/pr_volmaxmin`, `whifun_functions/whifun_paint.m:1/whifun_paint`, `whifun_functions/whifun_paint.m:361/sf_slice2panel`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `whifun_functions/private/pr_volmaxmin.m:1/pr_volmaxmin`, `whifun_functions/whifun_paint.m:1/whifun_paint`, `whifun_functions/whifun_paint.m:361/sf_slice2panel`

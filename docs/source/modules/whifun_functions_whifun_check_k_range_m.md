# Module Name: `whifun_functions/whifun_check_k_range.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Key Features:**
  - Written by Pratik Jain WHIFUN_CHECK_K_RANGE Checks the validity of a K-range. WHIFUN_CHECK_K_RANGE(K_range_l, K_range_h) verifies that the lower bound of a K-range (`K_range_l`) is less than or equal to the upper bound (`K_range_h`). If the condition `K_range_l > K_range_h` is met, the function generates an error and stops the script's execution. This is a crucial check to ensure that range-based parameters are specified in the correct order. Input Arguments: K_range_l - The lower bound of the K-range. K_range_h - The upper bound of the K-range. Example: % This will pass without error whifun_c
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_check_k_range()`

### Syntax
```matlab
function whifun_check_k_range(K_range_l,K_range_h)
```
Defined at source line `1`.

### Description
Written by Pratik Jain WHIFUN_CHECK_K_RANGE Checks the validity of a K-range. WHIFUN_CHECK_K_RANGE(K_range_l, K_range_h) verifies that the lower bound of a K-range (`K_range_l`) is less than or equal to the upper bound (`K_range_h`). If the condition `K_range_l > K_range_h` is met, the function generates an error and stops the script's execution. This is a crucial check to ensure that range-based parameters are specified in the correct order. Input Arguments: K_range_l - The lower bound of the K-range. K_range_h - The upper bound of the K-range. Example: % This will pass without error whifun_check_k_range(2, 10); % This will throw an error % whifun_check_k_range(10, 2); See also SPRINTF, ERR

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `K_range_l` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `K_range_h` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Tips
Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

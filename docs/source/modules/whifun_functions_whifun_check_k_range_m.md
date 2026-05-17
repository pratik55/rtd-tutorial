# Module Name: `whifun_functions/whifun_check_k_range.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Key Features:**
  - Written by Pratik Jain WHIFUN_CHECK_K_RANGE Checks the validity of a K-range. WHIFUN_CHECK_K_RANGE(K_range_l, K_range_h) verifies that the lower bound of a K-range (`K_range_l`) is less than or equal to the upper bound (`K_range_h`). If the condition `K_range_l > K_range_h` is met, the function generates an error and stops the script's execution. This is a crucial check to ensure that range-based parameters are specified in the correct order. Input Arguments: K_range_l - The lower bound of the K-range. K_range_h - The upper bound of the K-range. Example: % This will pass without error whifun_c
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_check_k_range()`
- **Signature & Definition:** `function whifun_check_k_range(K_range_l,K_range_h)` (line 1)
- **Scientific Theory & Formulas:** No standalone mathematical model is implemented; this routine is a procedural wrapper, GUI helper, compatibility adapter, or file-format utility.
- **Functional Purpose:** Written by Pratik Jain WHIFUN_CHECK_K_RANGE Checks the validity of a K-range. WHIFUN_CHECK_K_RANGE(K_range_l, K_range_h) verifies that the lower bound of a K-range (`K_range_l`) is less than or equal to the upper bound (`K_range_h`). If the condition `K_range_l > K_range_h` is met, the function generates an error and stops the script's execution. This is a crucial check to ensure that range-based parameters are specified in the correct order. Input Arguments: K_range_l - The lower bound of the K-range. K_range_h - The upper bound of the K-range. Example: % This will pass without error whifun_check_k_range(2, 10); % This will throw an error % whifun_check_k_range(10, 2); See also SPRINTF, ERR
- **Arguments:**
  - `K_range_l` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `K_range_h` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

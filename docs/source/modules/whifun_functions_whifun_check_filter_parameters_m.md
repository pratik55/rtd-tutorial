# Module Name: `whifun_functions/whifun_check_filter_parameters.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response.
- **Key Features:**
  - Written by Pratik Jain WHIFUN_CHECK_FILTER_PARAMETERS Checks if filter cutoffs are correctly ordered. WHIFUN_CHECK_FILTER_PARAMETERS(filter_lp, filter_hp) checks if the low-pass filter cutoff frequency (`filter_lp`) is less than or equal to the high-pass filter cutoff frequency (`filter_hp`). If the condition `filter_lp > filter_hp` is met, the function throws an error with a descriptive message, halting script execution. This is a useful utility function for validating user input in signal processing scripts. Input Arguments: filter_lp - The low-pass filter cutoff frequency (e.g., 0.1). filte
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_check_filter_parameters()`
- **Signature & Definition:** `function whifun_check_filter_parameters(filter_lp,filter_hp)` (line 1)
- **Scientific Theory & Formulas:** Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response.
- **Functional Purpose:** Written by Pratik Jain WHIFUN_CHECK_FILTER_PARAMETERS Checks if filter cutoffs are correctly ordered. WHIFUN_CHECK_FILTER_PARAMETERS(filter_lp, filter_hp) checks if the low-pass filter cutoff frequency (`filter_lp`) is less than or equal to the high-pass filter cutoff frequency (`filter_hp`). If the condition `filter_lp > filter_hp` is met, the function throws an error with a descriptive message, halting script execution. This is a useful utility function for validating user input in signal processing scripts. Input Arguments: filter_lp - The low-pass filter cutoff frequency (e.g., 0.1). filter_hp - The high-pass filter cutoff frequency (e.g., 0.01). Example: % This will pass without error w
- **Arguments:**
  - `filter_lp` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `filter_hp` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

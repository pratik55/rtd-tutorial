# Module Name: `whifun_functions/whifun_check_filter_parameters.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response.
- **Key Features:**
  - Written by Pratik Jain WHIFUN_CHECK_FILTER_PARAMETERS Checks if filter cutoffs are correctly ordered. WHIFUN_CHECK_FILTER_PARAMETERS(filter_lp, filter_hp) checks if the low-pass filter cutoff frequency (`filter_lp`) is less than or equal to the high-pass filter cutoff frequency (`filter_hp`). If the condition `filter_lp > filter_hp` is met, the function throws an error with a descriptive message, halting script execution. This is a useful utility function for validating user input in signal processing scripts. Input Arguments: filter_lp - The low-pass filter cutoff frequency (e.g., 0.1). filte
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_check_filter_parameters()`

### Syntax
```matlab
function whifun_check_filter_parameters(filter_lp,filter_hp)
```
Defined at source line `1`.

### Description
Written by Pratik Jain WHIFUN_CHECK_FILTER_PARAMETERS Checks if filter cutoffs are correctly ordered. WHIFUN_CHECK_FILTER_PARAMETERS(filter_lp, filter_hp) checks if the low-pass filter cutoff frequency (`filter_lp`) is less than or equal to the high-pass filter cutoff frequency (`filter_hp`). If the condition `filter_lp > filter_hp` is met, the function throws an error with a descriptive message, halting script execution. This is a useful utility function for validating user input in signal processing scripts. Input Arguments: filter_lp - The low-pass filter cutoff frequency (e.g., 0.1). filter_hp - The high-pass filter cutoff frequency (e.g., 0.01). Example: % This will pass without error w

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `filter_lp` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `filter_hp` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response.

### Tips
Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

# Module Name: `whifun_functions/whifun_plot_freqz.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - WHIFUN_PLOT_FREQZ Plots the frequency response of a digital filter. WHIFUN_PLOT_FREQZ(b, a, Fs) generates a two-part plot showing the magnitude and phase response of a digital filter. This function is a utility for visualizing the characteristics of a filter, such as a Butterworth bandpass filter used in fMRI preprocessing. The function uses MATLAB's `freqz` function to calculate the frequency response and then plots the magnitude (how much the filter amplifies or attenuates a given frequency) and phase (the phase shift applied to a frequency). The frequency axis is displayed in Hz. Input Argu
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: Signal Processing Toolbox

## `whifun_plot_freqz()`

### Syntax
```matlab
function whifun_plot_freqz(b,a,Fs)
```
Defined at source line `1`.

### Description
WHIFUN_PLOT_FREQZ Plots the frequency response of a digital filter. WHIFUN_PLOT_FREQZ(b, a, Fs) generates a two-part plot showing the magnitude and phase response of a digital filter. This function is a utility for visualizing the characteristics of a filter, such as a Butterworth bandpass filter used in fMRI preprocessing. The function uses MATLAB's `freqz` function to calculate the frequency response and then plots the magnitude (how much the filter amplifies or attenuates a given frequency) and phase (the phase shift applied to a frequency). The frequency axis is displayed in Hz. Input Arguments: b - The numerator coefficients of the filter transfer function. a - The denominator coefficie

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `b` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `a` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Fs` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** Signal Processing Toolbox
- **Called By:** `whifun_functions/whifun_qc_filter.m:1/whifun_qc_filter`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `whifun_functions/whifun_qc_filter.m:1/whifun_qc_filter`

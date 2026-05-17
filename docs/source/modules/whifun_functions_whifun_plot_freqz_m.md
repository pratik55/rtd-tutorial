# Module Name: `whifun_functions/whifun_plot_freqz.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - WHIFUN_PLOT_FREQZ Plots the frequency response of a digital filter. WHIFUN_PLOT_FREQZ(b, a, Fs) generates a two-part plot showing the magnitude and phase response of a digital filter. This function is a utility for visualizing the characteristics of a filter, such as a Butterworth bandpass filter used in fMRI preprocessing. The function uses MATLAB's `freqz` function to calculate the frequency response and then plots the magnitude (how much the filter amplifies or attenuates a given frequency) and phase (the phase shift applied to a frequency). The frequency axis is displayed in Hz. Input Argu
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: Signal Processing Toolbox

## Function: `whifun_plot_freqz()`
- **Signature & Definition:** `function whifun_plot_freqz(b,a,Fs)` (line 1)
- **Scientific Theory & Formulas:** Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** WHIFUN_PLOT_FREQZ Plots the frequency response of a digital filter. WHIFUN_PLOT_FREQZ(b, a, Fs) generates a two-part plot showing the magnitude and phase response of a digital filter. This function is a utility for visualizing the characteristics of a filter, such as a Butterworth bandpass filter used in fMRI preprocessing. The function uses MATLAB's `freqz` function to calculate the frequency response and then plots the magnitude (how much the filter amplifies or attenuates a given frequency) and phase (the phase shift applied to a frequency). The frequency axis is displayed in Hz. Input Arguments: b - The numerator coefficients of the filter transfer function. a - The denominator coefficie
- **Arguments:**
  - `b` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `a` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `Fs` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: Signal Processing Toolbox
  - Called By: `whifun_functions/whifun_qc_filter.m:1/whifun_qc_filter`
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

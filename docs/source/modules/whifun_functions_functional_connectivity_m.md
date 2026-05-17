# Module Name: `whifun_functions/functional_connectivity.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Fisher transformation uses $z=\operatorname{atanh}(r)=\frac{1}{2}\ln\frac{1+r}{1-r}$.
- **Key Features:**
  - FUNCTIONAL_CONNECTIVITY Calculates Functional Connectivity (FC) from averaged ROI time series. [VEC, NAN_SUB] = FUNCTIONAL_CONNECTIVITY(REG_TS, Z, WIN, STRIDE, NL) Computes static or dynamic functional connectivity matrices (Pearson correlation or Non-linear Xi correlation) and returns the unique upper-triangle elements as a vector. Input Arguments: REG_TS - Time series of the ROIs. Expected dimensions: T x ROI x Subj (Time points x Number of ROIs x Number of Subjects). Z - (Optional, default 0) Flag for Fisher Z-transformation: Z = 1: Apply Fisher Z-transformation to Pearson correlation resul
  - Internal calls detected: `corrvec`
  - External dependencies detected: Statistics and Machine Learning Toolbox, Parallel Computing Toolbox

## Function: `functional_connectivity()`
- **Signature & Definition:** `function [vec,nan_sub] = functional_connectivity(reg_ts,Z,win,stride,nl)` (line 1)
- **Scientific Theory & Formulas:** Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Fisher transformation uses $z=\operatorname{atanh}(r)=\frac{1}{2}\ln\frac{1+r}{1-r}$.
- **Functional Purpose:** FUNCTIONAL_CONNECTIVITY Calculates Functional Connectivity (FC) from averaged ROI time series. [VEC, NAN_SUB] = FUNCTIONAL_CONNECTIVITY(REG_TS, Z, WIN, STRIDE, NL) Computes static or dynamic functional connectivity matrices (Pearson correlation or Non-linear Xi correlation) and returns the unique upper-triangle elements as a vector. Input Arguments: REG_TS - Time series of the ROIs. Expected dimensions: T x ROI x Subj (Time points x Number of ROIs x Number of Subjects). Z - (Optional, default 0) Flag for Fisher Z-transformation: Z = 1: Apply Fisher Z-transformation to Pearson correlation results. Z = 0: Do not apply transformation. WIN - (Optional, default T) Window size for Dynamic Function
- **Arguments:**
  - `reg_ts` (numeric time-series matrix, commonly T x R, V x T, or T x R x S): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `Z` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `win` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `stride` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `nl` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `vec` (numeric scalar, vector, matrix, or multidimensional array): Output produced by the MATLAB implementation.
  - `nan_sub` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `corrvec`
  - External: Statistics and Machine Learning Toolbox, Parallel Computing Toolbox
  - Called By: `whifun_functions/whifun_create_avg_ts.m:1/whifun_create_avg_ts`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering.

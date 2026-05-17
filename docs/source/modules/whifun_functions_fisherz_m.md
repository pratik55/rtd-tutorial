# Module Name: `whifun_functions/fisherZ.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Fisher transformation uses $z=\operatorname{atanh}(r)=\frac{1}{2}\ln\frac{1+r}{1-r}$.
- **Key Features:**
  - FISHERZ Applies the Fisher's r-to-z transformation to correlation coefficients. Z = FISHERZ(R) The Fisher transformation (often called Fisher's Z-transformation) is used to transform the sampling distribution of the Pearson correlation coefficient (r) from a non-normal (skewed) distribution to a distribution that is approximately normal. This makes the transformed variable Z more suitable for statistical inference, such as calculating confidence intervals or performing hypothesis tests on correlation coefficients. The formula for the transformation is: $$Z = \frac{1}{2} \ln \left( \frac{1+r}{1
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `fisherZ()`

### Syntax
```matlab
function Z = fisherZ(r)
```
Defined at source line `1`.

### Description
FISHERZ Applies the Fisher's r-to-z transformation to correlation coefficients. Z = FISHERZ(R) The Fisher transformation (often called Fisher's Z-transformation) is used to transform the sampling distribution of the Pearson correlation coefficient (r) from a non-normal (skewed) distribution to a distribution that is approximately normal. This makes the transformed variable Z more suitable for statistical inference, such as calculating confidence intervals or performing hypothesis tests on correlation coefficients. The formula for the transformation is: $$Z = \frac{1}{2} \ln \left( \frac{1+r}{1-r} \right)$$ Input Arguments: R - The Pearson correlation coefficient(s) (or any value between -1 a

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `r` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Z` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

### More About
Fisher transformation uses $z=\operatorname{atanh}(r)=\frac{1}{2}\ln\frac{1+r}{1-r}$.

### Tips
Handles NaN, Inf, or finite-value filtering.

### Algorithms
Fisher transformation uses $z=\operatorname{atanh}(r)=\frac{1}{2}\ln\frac{1+r}{1-r}$.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

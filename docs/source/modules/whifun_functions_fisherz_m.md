# Module Name: `whifun_functions/fisherZ.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Fisher transformation uses $z=\operatorname{atanh}(r)=\frac{1}{2}\ln\frac{1+r}{1-r}$.
- **Key Features:**
  - FISHERZ Applies the Fisher's r-to-z transformation to correlation coefficients. Z = FISHERZ(R) The Fisher transformation (often called Fisher's Z-transformation) is used to transform the sampling distribution of the Pearson correlation coefficient (r) from a non-normal (skewed) distribution to a distribution that is approximately normal. This makes the transformed variable Z more suitable for statistical inference, such as calculating confidence intervals or performing hypothesis tests on correlation coefficients. The formula for the transformation is: $$Z = \frac{1}{2} \ln \left( \frac{1+r}{1
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `fisherZ()`
- **Signature & Definition:** `function Z = fisherZ(r)` (line 1)
- **Scientific Theory & Formulas:** Fisher transformation uses $z=\operatorname{atanh}(r)=\frac{1}{2}\ln\frac{1+r}{1-r}$.
- **Functional Purpose:** FISHERZ Applies the Fisher's r-to-z transformation to correlation coefficients. Z = FISHERZ(R) The Fisher transformation (often called Fisher's Z-transformation) is used to transform the sampling distribution of the Pearson correlation coefficient (r) from a non-normal (skewed) distribution to a distribution that is approximately normal. This makes the transformed variable Z more suitable for statistical inference, such as calculating confidence intervals or performing hypothesis tests on correlation coefficients. The formula for the transformation is: $$Z = \frac{1}{2} \ln \left( \frac{1+r}{1-r} \right)$$ Input Arguments: R - The Pearson correlation coefficient(s) (or any value between -1 a
- **Arguments:**
  - `r` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `Z` (numeric scalar or numeric vector): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Handles NaN, Inf, or finite-value filtering.

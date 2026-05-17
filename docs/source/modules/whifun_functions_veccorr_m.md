# Module Name: `whifun_functions/veccorr.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$.
- **Key Features:**
  - VECCORR Converts a vectorized upper-triangular matrix back into a full square matrix. MAT = VECCORR(VEC) This function reconstructs a symmetric matrix (e.g., a correlation matrix) from its compact vector representation of the unique upper-off-diagonal elements. Input Arguments: VEC - The input vector or matrix containing the vectorized upper-off-diagonal elements. Expected dimensions: (N*(N-1)/2) x S, where N is the number of regions/ROIs and S is the number of matrices (e.g., subjects, windows). Output Arguments: MAT - The reconstructed full matrix (or stack of matrices). Expected dimensions:
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `veccorr()`
- **Signature & Definition:** `function mat = veccorr(vec)` (line 1)
- **Scientific Theory & Formulas:** Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$.
- **Functional Purpose:** VECCORR Converts a vectorized upper-triangular matrix back into a full square matrix. MAT = VECCORR(VEC) This function reconstructs a symmetric matrix (e.g., a correlation matrix) from its compact vector representation of the unique upper-off-diagonal elements. Input Arguments: VEC - The input vector or matrix containing the vectorized upper-off-diagonal elements. Expected dimensions: (N*(N-1)/2) x S, where N is the number of regions/ROIs and S is the number of matrices (e.g., subjects, windows). Output Arguments: MAT - The reconstructed full matrix (or stack of matrices). Expected dimensions: N x N x S. The diagonal elements are set to NaN. Derivation of N (Number of Regions): The number of
- **Arguments:**
  - `vec` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `mat` (numeric scalar, vector, matrix, or multidimensional array): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: `whifun_statistics.mlapp:1174/plots_for_pairs`, `whifun_statistics.mlapp:986/plot_t`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files.

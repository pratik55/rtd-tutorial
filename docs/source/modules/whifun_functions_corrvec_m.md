# Module Name: `whifun_functions/corrvec.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps.
- **Key Features:**
  - CORRVEC Extracts the unique upper-triangular elements of a 2D or 3D correlation/adjacency matrix. CORR = CORRVEC(MAT, D) This function is primarily used to convert symmetric matrices (like correlation matrices or adjacency matrices) into a compact vector representation, which is often necessary before feeding data into clustering or multivariate statistical algorithms. Input Arguments: MAT - The input matrix (or matrices). - If 2D (N x N): A single symmetric matrix (e.g., a connectivity map). - If 3D (N x N x S): A stack of S symmetric matrices (e.g., dynamic FC windows, or multiple subjects).
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: Statistics and Machine Learning Toolbox

## Function: `corrvec()`
- **Signature & Definition:** `function Corr = corrvec(mat,d)` (line 1)
- **Scientific Theory & Formulas:** Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps.
- **Functional Purpose:** CORRVEC Extracts the unique upper-triangular elements of a 2D or 3D correlation/adjacency matrix. CORR = CORRVEC(MAT, D) This function is primarily used to convert symmetric matrices (like correlation matrices or adjacency matrices) into a compact vector representation, which is often necessary before feeding data into clustering or multivariate statistical algorithms. Input Arguments: MAT - The input matrix (or matrices). - If 2D (N x N): A single symmetric matrix (e.g., a connectivity map). - If 3D (N x N x S): A stack of S symmetric matrices (e.g., dynamic FC windows, or multiple subjects). D - (Optional, default 0) Flag to determine whether to include the diagonal elements (the self-corr
- **Arguments:**
  - `mat` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `d` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `Corr` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: Statistics and Machine Learning Toolbox
  - Called By: `whifun_functions/functional_connectivity.m:1/functional_connectivity`, `whifun_statistics.mlapp:132/WM_ttest`, `whifun_statistics.mlapp:614/Atlas_based_ttest`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files.

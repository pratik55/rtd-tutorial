# Module Name: `whifun_functions/whifun_nmi.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Normalized mutual information is $NMI=\frac{2I(X;Y)}{H(X)+H(Y)}$, where $I(X;Y)=\sum_{ij}p_{ij}\log_2\frac{p_{ij}}{p_i p_j}$.
- **Key Features:**
  - WHIFUN_NMI Calculates the Normalized Mutual Information (NMI) between two label vectors. nmi = WHIFUN_NMI(labels1, labels2) computes the Normalized Mutual Information between two vectors of cluster or classification labels. NMI is a symmetry measure of similarity between two data clusterings, ranging from 0 (no mutual dependence) to 1 (perfect correlation). This function is commonly used to evaluate the quality of a clustering algorithm by comparing its output (labels1) to known ground truth labels (labels2), or to compare two different clustering solutions. The calculation involves the follow
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: Statistics and Machine Learning Toolbox

## Function: `whifun_nmi()`
- **Signature & Definition:** `function nmi = whifun_nmi(labels1, labels2)` (line 1)
- **Scientific Theory & Formulas:** K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Normalized mutual information is $NMI=\frac{2I(X;Y)}{H(X)+H(Y)}$, where $I(X;Y)=\sum_{ij}p_{ij}\log_2\frac{p_{ij}}{p_i p_j}$.
- **Functional Purpose:** WHIFUN_NMI Calculates the Normalized Mutual Information (NMI) between two label vectors. nmi = WHIFUN_NMI(labels1, labels2) computes the Normalized Mutual Information between two vectors of cluster or classification labels. NMI is a symmetry measure of similarity between two data clusterings, ranging from 0 (no mutual dependence) to 1 (perfect correlation). This function is commonly used to evaluate the quality of a clustering algorithm by comparing its output (labels1) to known ground truth labels (labels2), or to compare two different clustering solutions. The calculation involves the following steps: 1. **Confusion Matrix (C)**: Creates a contingency table showing the overlap between the 
- **Arguments:**
  - `labels1` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `labels2` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `nmi` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: Statistics and Machine Learning Toolbox
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Handles NaN, Inf, or finite-value filtering.

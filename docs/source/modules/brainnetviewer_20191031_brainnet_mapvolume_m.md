# Module Name: `BrainNetViewer_20191031/BrainNet_MapVolume.m`
- **Module Category:** Bundled BrainNetViewer dependency.
- **Theoretical Background:** K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Normalized mutual information is $NMI=\frac{2I(X;Y)}{H(X)+H(Y)}$, where $I(X;Y)=\sum_{ij}p_{ij}\log_2\frac{p_{ij}}{p_i p_j}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - function rest_CallBrainNetViewer(BrainVolume,NMin,PMin,ClusterSize,ConnectivityCriterion,SurfFileName,viewtype,ColorMap,NMax,PMax,BrainHeader) Function to call BrainNet Viewer (by Mingrui Xia) by REST Slice Viewer. Also can be used to scripting call BrainNet Viewer. Input: BrainVolume - 1) The 3D Brain Volume (could be thresholded), parameter 'BrainHeader' needed. or 2) the File Name of a Brain Image, e.g. '/home/T.img' NMin - The negative minimum (minimum in absolute value). Could be the negative threshold - default: calculate from BrainVolume PMin - The positive minimum. Could be the positiv
  - Internal calls detected: `BrainNet`
  - External dependencies detected: SPM12, BrainNet Viewer

## Function: `BrainNet_MapVolume()`
- **Signature & Definition:** `function H_BrainNet = BrainNet_MapVolume(BrainVolume,NMin,PMin,ClusterSize,ConnectivityCriterion,SurfFileName,viewtype,ColorMap,NMax,PMax,BrainHeader)` (line 1)
- **Scientific Theory & Formulas:** K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Normalized mutual information is $NMI=\frac{2I(X;Y)}{H(X)+H(Y)}$, where $I(X;Y)=\sum_{ij}p_{ij}\log_2\frac{p_{ij}}{p_i p_j}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** function rest_CallBrainNetViewer(BrainVolume,NMin,PMin,ClusterSize,ConnectivityCriterion,SurfFileName,viewtype,ColorMap,NMax,PMax,BrainHeader) Function to call BrainNet Viewer (by Mingrui Xia) by REST Slice Viewer. Also can be used to scripting call BrainNet Viewer. Input: BrainVolume - 1) The 3D Brain Volume (could be thresholded), parameter 'BrainHeader' needed. or 2) the File Name of a Brain Image, e.g. '/home/T.img' NMin - The negative minimum (minimum in absolute value). Could be the negative threshold - default: calculate from BrainVolume PMin - The positive minimum. Could be the positive threshold - default: calculate from BrainVolume ClusterSize - Set a cluster (voxel number) must be
- **Arguments:**
  - `BrainVolume` (numeric image/header data, commonly X x Y x Z or X x Y x Z x T): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `NMin` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `PMin` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `ClusterSize` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `ConnectivityCriterion` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `SurfFileName` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `viewtype` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `ColorMap` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `NMax` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `PMax` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `BrainHeader` (numeric image/header data, commonly X x Y x Z or X x Y x Z x T): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `H_BrainNet` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `BrainNet`
  - External: SPM12, BrainNet Viewer
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering.

## Function: `AdjustColorMap()`
- **Signature & Definition:** `function NewColorMap=AdjustColorMap(OriginalColorMap,NullColor,NMax,NMin,PMin,PMax)` (line 152)
- **Scientific Theory & Formulas:** Normalized mutual information is $NMI=\frac{2I(X;Y)}{H(X)+H(Y)}$, where $I(X;Y)=\sum_{ij}p_{ij}\log_2\frac{p_{ij}}{p_i p_j}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** Adjust the colormap to leave blank to values under threshold, the orginal color map with be set into [NMax NMin] and [PMin PMax]. Written by YAN Chao-Gan, 111023 Input: OriginalColorMap - the original color map NullColor - The values between NMin and PMin will be set to this color (leave blank) NMax, NMin, PMin, PMax - set the axis of colorbar (the orginal color map with be set into [NMax NMin] and [PMin PMax]) Output: NewColorMap - the generated color map, a 1000 by 3 matrix.
- **Arguments:**
  - `OriginalColorMap` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `NullColor` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `NMax` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `NMin` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `PMin` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `PMax` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `NewColorMap` (numeric scalar, vector, matrix, or multidimensional array): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `AFNI_ColorMap()`
- **Signature & Definition:** `function ColorMap =AFNI_ColorMap(SegmentNum)` (line 193)
- **Scientific Theory & Formulas:** Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** Generate the color map like AFNI. Written by YAN Chao-Gan, 090601 Input: SegmentNum - the number of segments. it should be 2,4,6,8,9,10,11,12,13,14,15,16,17,18,19,20 or 256 Output: ColorMap - the generated color map, an x by 3 matrix.
- **Arguments:**
  - `SegmentNum` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `ColorMap` (numeric scalar, vector, matrix, or multidimensional array): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

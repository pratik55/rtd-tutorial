# Module Name: `whifun_functions/whifun_dartel_normalize_smooth.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - % Dartel - Normalize and Smooth output_folder = 'C:\Users\jainp\Box\practice_NY_op_home_laptop'; load(fullfile(output_folder,'parameters.mat')); Subj_list = load_subjects(output_folder,'Subj_list.csv'); Cut_pre = 'c_'; % Prefix for the Discarding Initial volumes File Realign_pre = 'r'; % Prefix for the Realignment File skull_pre = 'b'; % Prefix for the Skull Stripped File Reg_pre = 'REG_'; % Prefix for the Regressed File vox = 3; % Voxel Size of the Normalized (MNI) space f_pre = 'f'; % prefix for filtered file Norm_pre = 'w'; % Prefix for the Normalized File Smooth_pre = 's'; % Prefix for the
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: MATLAB table/file I/O, SPM12, Shell/system execution

## `whifun_dartel_normalize_smooth()`

### Syntax
```matlab
function output = whifun_dartel_normalize_smooth(Subj_list,func_anat,Smooth_pre,f_pre,Reg_pre,Realign_pre,Cut_pre,skull_pre,output_folder,vox)
```
Defined at source line `18`.

### Description
% Dartel - Normalize and Smooth output_folder = 'C:\Users\jainp\Box\practice_NY_op_home_laptop'; load(fullfile(output_folder,'parameters.mat')); Subj_list = load_subjects(output_folder,'Subj_list.csv'); Cut_pre = 'c_'; % Prefix for the Discarding Initial volumes File Realign_pre = 'r'; % Prefix for the Realignment File skull_pre = 'b'; % Prefix for the Skull Stripped File Reg_pre = 'REG_'; % Prefix for the Regressed File vox = 3; % Voxel Size of the Normalized (MNI) space f_pre = 'f'; % prefix for filtered file Norm_pre = 'w'; % Prefix for the Normalized File Smooth_pre = 's'; % Prefix for the

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `Subj_list` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `func_anat` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Smooth_pre` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `f_pre` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Reg_pre` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Realign_pre` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Cut_pre` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `skull_pre` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `output_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `vox` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `output` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** SPM12, Shell/system execution
- **Called By:** `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`

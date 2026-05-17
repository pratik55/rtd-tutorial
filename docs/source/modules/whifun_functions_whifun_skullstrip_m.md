# Module Name: `whifun_functions/whifun_skullstrip.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_SKULLSTRIP Performs SPM-based skull stripping using imcalc. output = WHIFUN_SKULLSTRIP(m_file, now_anat_path, skull_pre) creates a skull-stripped version of a bias-corrected anatomical image by using SPM's `imcalc` function. The function performs the following steps: 1. **Selects Inputs**: It takes the bias-corrected anatomical image (`m_file` , (`i1`)) and the native-space segmented images for Gray Matter (`c1`), White Matter (`c2`), and CSF (`c3`) as input. 2. **Defines the Expression**: It applies a logical expression `i1.*((i2+i3+i4)>0.5)` to the input images. This expression perfor
  - Internal calls detected: `complete_filepath`
  - External dependencies detected: SPM12, Shell/system execution

## `whifun_skullstrip()`

### Syntax
```matlab
function output = whifun_skullstrip(m_file,now_anat_path,skull_pre)
```
Defined at source line `1`.

### Description
WHIFUN_SKULLSTRIP Performs SPM-based skull stripping using imcalc. output = WHIFUN_SKULLSTRIP(m_file, now_anat_path, skull_pre) creates a skull-stripped version of a bias-corrected anatomical image by using SPM's `imcalc` function. The function performs the following steps: 1. **Selects Inputs**: It takes the bias-corrected anatomical image (`m_file` , (`i1`)) and the native-space segmented images for Gray Matter (`c1`), White Matter (`c2`), and CSF (`c3`) as input. 2. **Defines the Expression**: It applies a logical expression `i1.*((i2+i3+i4)>0.5)` to the input images. This expression performs an element-wise multiplication (`.*`) of the anatomical image (`i1`) with a binary mask. The mask

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `m_file` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `now_anat_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `skull_pre` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `output` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `complete_filepath`
- **External Dependencies:** SPM12, Shell/system execution
- **Called By:** `whifun_functions/whifun_skull_strip_and_anat_mask_preproc.m:1/whifun_skull_strip_and_anat_mask_preproc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `complete_filepath`
- Related callers: `whifun_functions/whifun_skull_strip_and_anat_mask_preproc.m:1/whifun_skull_strip_and_anat_mask_preproc`

# Module Name: `whifun_functions/whifun_count_file_patterns.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_COUNT_FILE_PATTERNS Audits dataset structure by counting file naming patterns. Author: Pratik Jain This function recursively scans a directory and identifies unique file naming patterns by abstracting subject-specific IDs (sub-XXXX) into wildcards (sub*). It is designed to validate BIDS-compliant datasets. INPUTS: dataset_path - String. The root directory of your fMRI dataset. OUTPUTS: pattern_table - A table containing: * Name: The abstracted file path and pattern. * Value: The total count of files matching that pattern. EXAMPLE: % Check if all 20 subjects have their MNI-space bold fil
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_count_file_patterns()`

### Syntax
```matlab
function pattern_table = whifun_count_file_patterns(dataset_path)
```
Defined at source line `1`.

### Description
WHIFUN_COUNT_FILE_PATTERNS Audits dataset structure by counting file naming patterns. Author: Pratik Jain This function recursively scans a directory and identifies unique file naming patterns by abstracting subject-specific IDs (sub-XXXX) into wildcards (sub*). It is designed to validate BIDS-compliant datasets. INPUTS: dataset_path - String. The root directory of your fMRI dataset. OUTPUTS: pattern_table - A table containing: * Name: The abstracted file path and pattern. * Value: The total count of files matching that pattern. EXAMPLE: % Check if all 20 subjects have their MNI-space bold files audit = whifun_count_file_patterns('/data/project/derivatives/fmriprep'); See also DIR, REGEXPREP

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `dataset_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `pattern_table` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** `whifun_functions/whifun_plot_important.m:1/whifun_plot_important`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `whifun_functions/whifun_plot_important.m:1/whifun_plot_important`

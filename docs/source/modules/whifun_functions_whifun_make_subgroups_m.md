# Module Name: `whifun_functions/whifun_make_subgroups.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$.
- **Key Features:**
  - WHIFUN_MAKE_SUBGROUPS Creates minimal overlapping subgroups of subjects from a total pool. [SUBGROUPS, OVERLAPS] = WHIFUN_MAKE_SUBGROUPS(TOTAL_SUBJECTS, N) This function partitions a set of 'total_subjects' into subgroups of size 'n'. If the total number of subjects is not divisible by 'n', the last subgroup is formed by taking the remaining subjects and "filling" the group to size 'n' by randomly sampling subjects from the previously formed full subgroups. This ensures all subgroups are of uniform size 'n', but the last group may overlap with others. Input Arguments: TOTAL_SUBJECTS - The tota
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_make_subgroups()`

### Syntax
```matlab
function [subgroups, overlaps] = whifun_make_subgroups(total_subjects, n)
```
Defined at source line `1`.

### Description
WHIFUN_MAKE_SUBGROUPS Creates minimal overlapping subgroups of subjects from a total pool. [SUBGROUPS, OVERLAPS] = WHIFUN_MAKE_SUBGROUPS(TOTAL_SUBJECTS, N) This function partitions a set of 'total_subjects' into subgroups of size 'n'. If the total number of subjects is not divisible by 'n', the last subgroup is formed by taking the remaining subjects and "filling" the group to size 'n' by randomly sampling subjects from the previously formed full subgroups. This ensures all subgroups are of uniform size 'n', but the last group may overlap with others. Input Arguments: TOTAL_SUBJECTS - The total number of subjects available (e.g., number of rows in a data table). N - The desired size of each

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `total_subjects` — numeric time-series matrix, commonly T x R, V x T, or T x R x S
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `n` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `subgroups` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

#### `overlaps` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$.

### Tips
Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

# OMQDI
Objective Measure of Quality of Denoised Images

This python module implements the Objective Quality Measure of Denoised Images, a no-reference image quality assessment metric developed for magnetic resonance images.

## Usage
```python
from IQA import OMQDI
omqdi_value, edge_preservation_factor, noise_suppression_factor = OMQDI(X, Y)
```

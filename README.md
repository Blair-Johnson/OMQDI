# OMQDI: Objective Measure of Quality of Denoised Images

This python module implements the Objective Quality Measure of Denoised Images, a no-reference image quality assessment metric developed for magnetic resonance images.

## Usage
Pass a single-channel 2D noisy image array and a denoised version to OMQDI. The order of images does not affect the result.
```python
from IQA import OMQDI
X = imread(noisey.png)
Y = imread(denoised.png)
omqdi_value, edge_preservation_factor, noise_suppression_factor = OMQDI(X, Y)
```

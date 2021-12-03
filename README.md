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
![Example Images](https://github.com/Blair-Johnson/OMQDI/blob/main/example.png?raw=true)

## Notes
The local variance calculation in this implementation differs from the original paper. The original paper cites an equation that is not equivalent to local variance (equation 6), and this results in erroneous noise suppression factor values.

## References
[1] V. R. Simi, D. Reddy Edla, and J. Joseph, “A no-reference metric to assess quality of denoising for Magnetic Resonance images,” Biomedical Signal Processing and Control, vol. 70, p. 102962, 2021, doi: 10.1016/j.bspc.2021.102962.
  


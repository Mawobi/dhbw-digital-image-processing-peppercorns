# DHBW Mosbach INF19X - Digital Image Processing

---

## Project

Management of a spice-processing factory is currently deciding whether to invest into a new camera system for visual inspection of spices.

The one in use is getting old and the images it captures are corrupted. However, even such corrupted data seems to be analyzable for the purposes of quality inspection.

Your task is to develop an algorithm in Python which will count the black peppercorns in the following input image.

The solution can be a pure python file or an ipynb file, but it must be runnable (meaning I will not need to do any imports, there will be no syntax errors, etc.).

For this, you may assume that the input image is in the same directory and use e.g. the following to read it:

```python
tifffile.imread('[input.tif](input.tif)')
```

## Notes

- **There are 110 peppercorns in the input image**
- Manual counting of peppercorns is not allowed, you will get points for your algorithm, which must count the peppercorns
- You cannot manually pre-process parts of the image (e.g. split peppercorns which appear merged by drawing a line between them). Imagine getting another image where the peppercorn distribution would be different, your algorithm should be applicable to that image too.
- Some helpful modules/functions:
  - numpy.fft
  - scipy.ndimage
  - skimage.morphology
  - skimage.measure.label
2024-06-1221:14
Tags:[[Data Augmentation]]
# Resize

- You can resize images with `Resize.squish` (Squishes the image) or others like pad with black or zeroes.
- All these methods have drawbacks. We may pick to instead randomly select a part of the image. `RandomResizedCrop`. This allows the same image to appear multiple times but different parts of it.
- This possibly makes our model better.



---
# References

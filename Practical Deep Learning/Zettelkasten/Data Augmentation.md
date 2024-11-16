2024-05-3110:24
Tags:[[Deep Learning]]
# Data Augmentation

- Synthetically generate variations of input images. This is done by applying transforms such as rotation, brightness change, stretching etc.
- For images, a set of augmentations is provided with the `aug_transforms` function 
> [!code]- aug_transforms : 
> ``` python
> Signature:
aug_transforms(mult: 'float' = 1.0,do_flip: 'bool' = True,flip_vert: 'bool' = False,max_rotate: 'float' = 10.0,min_zoom: 'float' = 1.0,max_zoom: 'float' = 1.1,max_lighting: 'float' = 0.2,max_warp: 'float' = 0.2,p_affine: 'float' = 0.75,p_lighting: 'float' = 0.75,xtra_tfms: 'list' = None,size: 'int | tuple' = None,mode: 'str' = 'bilinear',pad_mode='reflection',align_corners=True,batch=False,min_scale=1.0)```


---
# References
Ch 2. From Model to Production
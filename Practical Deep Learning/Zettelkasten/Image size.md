2024-05-0415:40
Tags:[[fastai]]
# Image size
- Normally we use 224 pixels for historical reasons. 
- However, we can pick any size. 
**Bigger size** = Slower, more memory use, more precise

`Resize` is a fastai function that resizes the images. Used with the item transform parameter in the DL dataset definition 
```python
dls = ImageDataLoaders.from_name_func(
... 
items_tfms = Resize(224)
...
)
```




---
# References
ch01_ Practical Deep Learning for Coders 
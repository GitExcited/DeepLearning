2024-06-1221:06
Tags:[[fastai]]
# DataBlock

- A *Template* for creating [[DataLoaders]] 
**Example**:
```python
bears= DataBlock(
    blocks=(ImageBlock,CategoryBlock),#independant, dependant variables
    get_items=get_image_files,#how to find path to images
    splitter=RandomSplitter(valid_pct=0.2,seed=42),#how to define the validation set
    get_y=parent_label,#parent_label is a fastai func. set dependant variable to parent folder name
    item_tfms=Resize(128)#images are sent in batches as a tensor. tfo must resize them to be similar
)
```


 
---
# References
Ch 02 From Model to Production
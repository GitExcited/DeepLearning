2024-06-1021:25
Tags:[[fastai]]
# DataLoaders
> Class that stores the DataLoader object you pass to it
```python
class DataLoaders(GetAttr):
	def __init__(self, *loaders): self.loaders = loaders
	def __getitem__(self, i): return self.loaders[i]
	train,valid = add_props(lambda i, self: self[i])
```

To turn Data into `DataLoaders` we need to tell fastai:
- What **kinds of data** we are working with 
	- Ex: image and category 
- How to **get the list** of items
	- Ex: `get_image_files`
- How to **create the validation** set
	- Ex:`RandomSplitter( valid_pct = 0,2)`
- How to **label** these items 
	- Ex: `parent_label`

First a [[DataBlock]] is created then we tell fastai what is the path to our data. 
`dls = <<someDataBlock>>.dataloaders(path)`

## Methods
- **valid.showbatch()**
	- By default, 64 elements are put in a tensor and sent to the GPU at a time. To see what the batch looks like: 
	`<<someDataLoaders>>.valid.show_batch(max_n=4, nrows = 1)`
	


---
# References
Ch 02 From Model to Production


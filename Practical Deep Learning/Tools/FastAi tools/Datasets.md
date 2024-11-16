2024-10-1608:25
Tags:[[Datasets]][[fastai]]
# Datasets

Fastai has a lot of available datasets for Image classification, NLP, image localization, audio classification.

Also [[pretrained models]] like:
1. **OPENAI_TRANSFORMER**: The GPT2 Transformer pretrained weights.
2. **WT103_FWD**: The WikiText-103 forward language model weights.
3. **WT103_BWD**: The WikiText-103 backward language model weights.

### Open data
```python
path = untar_data(URLs.PETS)/'images'
#downloads data from URLs global constant used for datasets.
#PETS is the name of the dataset
#it is placed in a new path 'images'
```

---
# References
[List of datasets](https://docs.fast.ai/data.external.html#datasets)
[URLs and untar_data documentation](https://docs.fast.ai/data.external.html#urls)
2024-05-0416:12
Tags:[[architecture]] 
# pretrained models

- A model that has weights that have already been trained on some other dataset.
- You should **nearly always** use a pretrained model. It is already very capable with common capabilities such as recognition of :edges, colours, gradients. 
- When using pretrained model, the last layer is removed and replaced with one or more new layers with randomized weights. This part of the model is the [[head]] 
- Allow for quickly and cheaply training models.
- **Transfer learning**: using a pretrained model for a task different than it was originally trained for.
- In [[fastai]] we use [[fine_tune]] in order to *fit* a pretrained model


---
# References
CH 01 Deep Learning
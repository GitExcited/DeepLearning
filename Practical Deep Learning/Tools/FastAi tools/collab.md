2024-10-1509:50
Tags:[[fastai]]
# collab

Used to train [[Collaborative Filtering]] models. 

```python
from fastai.collab import*
path= untar_data(URLs.ML_SAMPLE)
dls=CollabDataLoaders.from_csv(path/'ratings.csv')
``` 



---
# References

2024-05-0415:48
Tags:[[Deep Learning]]
# Validation Set
- The parameter `valid_pct` in [[fastai]] 
- Determines how much of the data is *not used for training the model at all*. 
- A validation and [[Test set]] must be representative of new data you will see in the future.
- The part that isn't training set is called the [[training set]]

>[!note]  [[fastai]] always shows you your model's accuracy using **only the validation set**. This is critical! If you train a model for long enough time, it will memorize the label of every item in your data. What we care about is if it is able to predict images it has not seen yet.



---
# References
Ch 1 Practical deep learning 
2024-05-0415:23
Tags:[[machine learning]]
# Limitations
- A model cannot be created without *data*
- A model can only learn with the patterns seen in the *data* used to train it
- The learning only creates *predictions*, not recommended actions.
- Input data must also have *labels* to be useful. Therefore [[labels is as important as data]]
- Deep learning algos have trouble recognizing images with different structure or style from those used in training (ex: black-and-white images might do poorly if none were used in training.)

# Potential problems
- *Positive feedback loops* occur when the more the model is used, the more biased the data becomes. 
>[!example]- Examples of Feedback loops:
>A model trained on where arrests have been made in the past to predict future crime. It leads to more arrests in the predicted zone, which feeds the model and continues to be biased towards a zone in the future versions in the model
>A model predicts video recommendation based on the biggest watchers or video. People who tend to binge watch are generally people who watch conspiracy theories. This results on more conspiracy theory videos being recommended which feeds into a loop in the model.

- [[Overfitting]]
- Models tend to gravitate towards the simplest way of ding good predictions: *Memorization*
- Erroneous context-appropriate NLP. Ex: a DL model might be able to summarize a text but its not guaranteed to be *correct*
- Bad Recommendations: Nearly all ML approaches tell you what the user might like rather what he might want to buy. Ex: if you buy lots of books from author A, you will keep getting recommended author A even though you already knew about this books. Instead of being recommended a similar author B.



---
# References
Ch 02 From Model to Production
2024-10-1610:05
Tags:[[Practical Deep Learning Book]]
# Chapter 1 PDL

[[machine learning]] is a discipline where we define a program not by writing it entirely ourselves, but by learning from data. [[Deep learning]] is a specialty within machine learning that uses [[Neural network]]s with multiple [[Network layer|layers]] . _Image classification_ is a representative example (also known as _image recognition_). We start with _labelled data_; that is, a set of images where we have assigned a _label_ to each image indicating what it represents. Our goal is to produce a program, called a _model_, which, given a new image, will make an accurate _prediction_ regarding what that new image represents.

Every model starts with a choice of _architecture_, a general template for how that kind of model works internally. The process of _training_ (or [[fit|fitting]]) the model is the process of finding a set of _parameter values_ (or _weights_) that specialize that general architecture into a model that works well for our particular kind of data. In order to define how well a model does on a single prediction, we need to define a _loss function_, which determines how we score a prediction as good or bad.

To make the training process go faster, we might start with a [[pretrained models]]—a model that has already been trained on someone else's data. We can then adapt it to our data by training it a bit more on our data, a process called [[fine_tune|fine-tuning]].

When we train a model, a key concern is to ensure that our model _generalizes_—that is, that it learns general lessons from our data which also apply to new items it will encounter, so that it can make good predictions on those items. The risk is that if we train our model badly, instead of learning general lessons it effectively memorizes what it has already seen, and then it will make poor predictions about new images. Such a failure is called [[Overfitting]]. In order to avoid this, we always divide our data into two parts, the [[training set]] and the [[Validation Set]]. We train the model by showing it only the training set and then we evaluate how well the model is doing by seeing how well it performs on items from the validation set. In this way, we check if the lessons the model learns from the training set are lessons that generalize to the validation set. In order for a person to assess how well the model is doing on the validation set overall, we define a _metric_. During the training process, when the model has seen every item in the training set, we call that an _epoch_.

All these concepts apply to machine learning in general. That is, they apply to all sorts of schemes for defining a model by training it with data. What makes deep learning distinctive is a particular class of architectures: the architectures based on [[Neural network]]. In particular, tasks like image classification rely heavily on [[convolutional neural network]]s, which we will discuss shortly.


---
# References

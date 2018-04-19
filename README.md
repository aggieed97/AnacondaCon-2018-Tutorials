# AnacondaCon 2018 Tutorials: Practical Data Science on ML with GPUs  

These notebooks were originally proved by Stan Seibert of Anaconda.  This was part of the tutorial series leading into AnacondaCon 2018 on Sunday, April 8th.  I had the fortune of being able to attend two tutorials, and this one was incredibly meaningful.  He was open to us downloading these notebooks and using them as we wish.  If there are any issues with posting these on my github, please contact me directly.  Unfortunately I noticed that many of the images originally created in Holoviews in the notebooks are no longer viewable; not sure how to fix this at the moment since they were pretty darn cool.  

This repository consists of five notebooks:

1. [Getting Started and Data Prep](#getting)
2. [Building and Training Models](#building)
3. [Evaluating Models](#evaluating)
4. [Saving a Model](#saving)
5. [Loading and Benchmarking](#loading)

### Getting Started and Data Prep
In this notebook Stan goes over the basic introductory material needed for the tutorial: the tools needed for Deep Learning, the recommended Hardware/OS requirements, and software requirements.  He also went into how he is loading and inspecting the CIFAR10 Data set provided with Keras.  He also rescales the data and uses One-Hot Encoding to transform the labels in the data set which has 10 categories.

### Building and Training Models
For this notebook, Stan creates his base model using Keras.  Since this is a multi-class problem, he using categorical_crossentropy as the loss function and Adadelta has the optimizer.  This goes against what we used in our Data Science Immersive Class since we were told to *always* use Adam as our optimizer.  Stan goes on to fit and train the model.  Unfortunately this is where Holoviews breaks down since it was pretty interesting to see the correct images versus what was predicted by the model.

### Evaluating Models
Here Stan demonstrates how to plot a confusion matrix to help evaluate our base model and how to control overfit with Dropout in the model.  He goes on to create a more complex model.  I really like his "looking at what others have done is your best intuition" line in regards to building a more complex model for your specific problem.  There really should not be any need to "re-invent the wheel" time and time again for a specific set of problems (i.e. image classification).  

### Saving a Model
In this notebook, Stan shows how to save a model for use in the future.  This saves time in having the run the model over and over again for future use (and for getting it ready for production).

### Loading and Benchmarking
For the last notebook, Stan shows how to load a trained model from disk, and then benchmark the performance of the model on the CPU and GPU used.

### Key Takeaways
I really enjoyed this tutorial.  There were several highlights to attending AnacondaCon 2018, and getting to go to this tutorial was easily one of those highlights.  There were lots of great talks some of which I would like to get more information on especially the newest rollout of Tensorflow 1.7, using Recurrent Neural Networks for Predictive Maintenance, using Machine Learning to Drive Sales, and using A/B Testing with Advanced Analytics.  It's unfortunate that I was only able to attend one day of conference besides the Tutorials, but I would certainly consider going next year if given the chance.


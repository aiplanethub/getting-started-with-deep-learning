# Introduction to Deep Learning

## Learning Objectives
* What and why Deep Learning?
* Machine Learning vs Deep Learning
* Deep Learning Applications
* Deep Learning Frameworks



## Some Cool Deep Learning Applications


### Flappy Bird
* A deep learning agent playing Flappy Bird!
* The agent is able to play without being told any information about the structure of the game or its rules.
* It automatically discovers the rules of the game by finding out how well it did each time. This approach is called Deep Reinforcement Learning.









![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_370f73818fa44ea18386ca0bbc6a67c9.png)











### Increasing the pixels of a blurry image
* Increase the resolution of a blurry image through deep learning.







![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_a34b5c4824c547c09cd62de74a1938d4.png)







### LipNet
* Lip reading performed more accurately than humans.











<iframe width="560" height="315" src="https://www.youtube.com/embed/fa5QGremQf8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>







## Why Deep Learning?
* Older machine learning algorithms typically plateau (become constant) in performance after they reach a threshold of data.
* Deep learning is one-of-a-kind algorithm whose performance continues to improve because more the data fed, the more the classifier is trained, resulting in outperforming the traditional models/ algorithms.









![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_069044c19a7a4bb0885f90f7e3e4da46.png)








## Deep Learning - An Analogy

Look at how a child learns language:

You show an apple to a kid and say “this is an apple”. Repeating it for 20 times, a connection in its brain is established and it can now recognize apples. What is important - at the beginning it can not differentiate small details. Small ball in your hand is going to be an apple because it follows the same pattern (small, rounded, red/green). Only an apple is rooted in a little brain.
The child points at an object and says, ‘apple.’ The child’s parent immediately provide feedback: ‘Right’ or ‘No, that’s a ball”.






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_cb492344be19473db6aa9c6e77ed0118.png)








Slowly, after enough feedback, the child eventually forms an internal mental model of how to label different objects in the world.

## What is Deep Learning?

A Deep Learning algorithm is able to learn hidden patterns from the data by itself (without human supervision), combine them together, and build much more efficient decision rules.

Now what does learning hidden patterns mean? Taking the same apple example, it means that:
* A deep learning model first identifies the low level features like the edges of an apple
* Then it slowly understands the more complex features like body and stem.
* Finally, it combines all the learnings and learns the shapes, colours and other characteristics that can be used to identify an apple.

The further you advance into it, the more complex the features it can
recognize.



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_2352add223d64d25b02a584024306a16.png)




## Machine Learning vs Deep Learning











![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_94374f0ae72040b29b1676739e349e81.png)











In practical terms, deep learning is just a subset of machine learning.

In fact, deep learning technically is machine learning and functions in a similar way (hence why the terms are sometimes loosely interchanged). However, its capabilities are different.

If you’ve worked with Machine Learning in the past, you might
have heard about Feature Extraction. What is it?

**Feature Extraction** means extracting the useful features of a dataset.
For eg. The stem and body of an apple.

* In traditional Machine learning techniques, most of the features need to be identified by an domain expert in order to reduce the complexity of the data and make patterns more visible for learning algorithms to work.  \
Unfortunately, feature extraction is a separate and often a manual component in machine learning pipeline and it is time-consuming.
* The biggest advantage of Deep Learning algorithms are that they try to learn features from data in an incremental manner. As discussed before, the model will first learn the basic constituents/low-level features before moving on to the high level ones i.e it learns on ITS OWN!

This eliminates the need of domain expertise and hard core feature extraction.

Have a look at the next figure to understand this better.
![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_c12e5356575941c0824b3b1636919765.png)


## Why is Deep Learning so popular?
In 2012, deep neural networks began to outperform traditional classification algorithms, including machine learning algorithms.

This is largely due to increased performance of computer processors (CPUs & GPUs) and larger storage media for retaining huge training datasets. Every year since, deep learning has continued to get better, becoming state of the art for solving problems in many different domains. This explosion in deep learning is largely thanks to improvements in hardware and massive labeled data sets that allow deep learning models to improve quickly over time.

Google trend for the keyword “Deep Learning”









![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_88fefb405fa3411dbd1a49158aa61198.png)









<iframe width="560" height="315" src="https://www.youtube.com/embed/yfsTZbwgMSE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>










## Deep Learning Applications in daily lives
### Social Media
One of the most common applications of Deep Learning is Automatic Friend Tagging Suggestions in Facebook or any other social media platform.

Facebook uses face detection and Image recognition to automatically find the face of the person which matches it’s Database and hence suggests us to tag that person based on DeepFace.

### Virtual Personal Assistants
Have you ever thought about what lies behind the working of Google Assistant, Siri or Alexa?

As the name suggests, Virtual Personal Assistants assist in finding useful information, when asked via text or voice. All you need to do is ask a simple question like “What is my schedule for tomorrow?” or “Show my upcoming Flights“.

Recently, personal assistants are being used in Chatbots which are being implemented in various food ordering apps, online training websites and also in Commuting apps. It is even used for shopping purposes.

### Healthcare
Deep learning provides the healthcare industry with the ability to analyze data at exceptional speeds without compromising on accuracy.

The technology has been applied across several other areas over the years. These include AI-powered chatbots that can identify patterns in patient symptoms, deep learning algorithms designed to identify certain cancers, pathology, and the identification of rare diseases.

Within each of these areas, deep learning plays a fundamental role in providing the medical professional with insights that allow them to identify issues early and provide highly personalized and relevant patient care.

### Other Applications
Apart from the ones you just saw, the number of deep learning applications in our daily lives are immense.

Can you think about more such applications?

Add them [here](https://discuss.dphi.tech/t/day-1-introduction-to-deep-learning/685).

## Deep Learning Frameworks

Both TensorFlow and PyTorch have their advantages as starting platforms to get into neural network programming.
Traditionally, researchers and Python enthusiasts have preferred PyTorch, while TensorFlow has long been the favored option for building large scale deep learning models for use in production.
However, the latest releases have seen the two libraries converge towards a more similar profile. As long as you stick to either TensorFlow or PyTorch as your deep learning framework, you can do nothing wrong.
Slide Download Link
You can download the slides here: https://docs.google.com/presentation/d/1XdenSAVaiFMdbtCqaG70y EHOdQLVr2ehnbQQPJDRo5E/edit?usp=sharing

That’s it for the day. Thank you!
Feel free to post any queries on Discuss or in the #help channel on Slack
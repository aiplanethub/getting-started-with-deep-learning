## Introduction to tf.Keras and Tensors

## Learning Objectives

* TensorFlow, Keras & tf.keras
* Setting up TensorFlow
* Tensors

#### TIP: You DON’T need to memorize the below jargons!

## TensorFlow, Keras and tf.keras

### What is TensorFlow?

* As you are aware by now, Tensorflow is a deep learning library/framework open-sourced by Google.
* It has grown to become one of the most loved and widely adopted
* ML platforms in the world.
* The TensorFlow community includes:
    * Researchers
    * Developers
    * Companies







![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_c838e53553cd416198883d0c338be31a.png)








### What & Why Keras?
* Keras is a deep learning API (a tool that enables two applications to exchange data among each other) written in Python.
* It runs on top of TensorFlow.
* It was developed with a focus on enabling fast experimentation. Being able to go from idea to result as fast as possible is the key to doing good research.






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_c1ce974a71d746028a86ee2fc031b4d0.png)







tf.keras is a Tensorflow-specific implementation of Keras. The name prefix “tf” itself says it is specific to the TensorFlow framework.

Since tf.keras is a specific implementation of TensorFlow, it has some advantages and supports many TensorFlow-specific features.

**History/context**: Not so long ago, on September 30th, 2019, Tensorflow 2.0 was launched. After the launch, developers started promoting something called tf.Keras.

### Keras vs. tf.Keras

We would suggest using TensorFlow 2.0 and tf.keras for future projects.

Not only you will enjoy the **added speed and optimization** of TensorFlow 2.0, but you’ll also receive **new feature updates** — the latest release of the Keras package (v2.3.0) will be the last release to support multiple backends and feature updates. Moving forward, the Keras package will receive only bug fixes.

### Tensorflow 2.0 Ecosystem & its use cases

Tensorflow 2.0 is not just a library, it’s an Ecosystem. Not only do you have the ability to train your own models using TensorFlow 2.0 and tf.keras, but you can now use:
* TensorFlow Lite: lightweight library for deploying models on mobile and embedded devices.
* TensorFlow Extended: end-to-end platform for preparing data, training, validating, and deploying models in large production environments.







![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_6ff5f9dca73c48108b4d4c972c086810.png)










Now that we know why we’re using Tensorflow 2.0 and tf.keras, let’s get started with it!

## Setting up Tensorflow

### Importing Tensorflow

Even if Tensorflow has been installed, we’ll always need to import it before use.

Within a Jupyter or Colab Notebook, you can import TensorFlow with a simple import statement. Just how we used np for numpy or pd for Pandas, we’ll be using tf for importing Tensorflow. Run this line of code to do this: `import tensorflow as tf`

On running this cell, TensorFlow will be imported and available for your use!
Cmeck tme verıion o² Tenıor²low

Open a Jupyter Notebook/Google Colab
In a cell type and execute the following command:

Make sure the displayed version starts with 2 i.e ensure
Tensorflow 2 has been installed.
Google Colab uses TensorFlow 2 by default.
Tensors
13
Wmy ımould we ıtudy about Tenıorı?
Tensors are the primary data structures used by neural
networks (the building blocks of Deep Learning).
And they are rather fascinating as well!
In neural networks transformations, input, output etc are performed via tensors.
Wmat are Tenıorı?

Wmat are Tenıorı?
Tensors are multi-dimensional arrays with a uniform type
(called a dtype).
If you're familiar with NumPy, tensors are (kind of) like
np.arrays.
All tensors are immutable like Python numbers and strings i.e you can never update the contents of a tensor, only create a new one.
Wmat are Tenıorı?
As you can see in the figure, the first 3 ranks of Tensors have special
names that you might have encountered in the past.
Rank 0 tensor - Scalar
Rank 1 tensor - Vector
Rank 2 tensor - Matrix
The tensors with ranks more than 2 are simply called ‘ Tensor ’.
Underıtanding Tenıor
How iı tme tenıor ımape important?
Our networks operate on tensors, after all, and this is why understanding a tensor’s shape and the available reshaping operations are super important.
Let’s learn about the shape and the methods of reshaping
tensors in the next 2 videos.
Note: These videos involve some syntax of PyTorch but not to worry, the concepts remain the same regardless of the framework! We have added a practical implementation of it in tensorflow provided in the github repository.
Rank, Axeı and Smape

Reımape, Squeeze and Flatten

Additional Reıourceı

On going through the below short resources from Tensorflow’s official documentation, you’ll notice the similarity between what you saw in the videos and what is implemented.
Tensorflow Reshape: https://docs.w3cub.com/tensorflow~python/tf/reshape/
Tensorflow Squeeze: https://docs.w3cub.com/tensorflow~python/tf/squeeze/
Let’s Practice

Tensorflow Operations Notebook:
https://github.com/dphi- official/Deep_Learning_Bootcamp/tree/master/Tensor_Operations
Slideı Download Link

You can download this module from the below link:
https://docs.google.com/presentation/d/1aFh443T4jAy6LVUv5BwPFhlig 7gAyq0IahAb4r-kd5Y/edit?usp=sharing

That’s it for the day. Thank you!
Feel free to post any queries in the #help channel on Slack
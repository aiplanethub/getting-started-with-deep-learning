## Learning Objectives

* Generative Adversarial Network (GAN)
* Autoencoders
* Neural Networks as Universal Approximators
* Recurrent Neural Network (RNN)
* Long Short-Term Memory (LSTM)
* Gated Recurrent Unit (GRU)


## Neural Networks as Universal Value Approximators

One of the most striking facts about neural networks is that they can compute any function out there!

Neural networks have a kind of universality. No matter what function we want to compute, we know that there is a neural network that can do the job. That is why they are known as Universal Value Approximators.

If you’re interested to learn more about it, this article gives a simple and mostly visual explanation of the universality theorem:

http://neuralnetworksanddeeplearning.com/chap4.html

Till now, you’ve worked with MLP and CNN, and that introduced you to the world of Deep Learning.

But what’s more out there? Let’s have a look!


## Recurrent Neural Network

Imagine that you are watching a movie. Most likely you would be able to connect to the scenes of the movie and understand what is happening, right? All our thinking goes in a flow and based on previous frame we can connect the current frame easily. Our thoughts have persistence.

Well, can we expect a neural network to make sense out of it? Not really!

Our traditional neural network architectures (Feed-forward neural networks) cannot do this. Given a particular sequence of frames, they cannot predict or understand what is happening at each point in the movie.

They have no memory of the input they receive and are bad at predicting what’s coming next. Because a feed-forward network only considers the current input, it has no understanding of sequence or time. It simply can’t remember anything about what happened in the past except its training.




![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_f1f5a2c614a34e5c88c8e59dd283b345.png)






This is where RNN comes in.

In an RNN the information cycles through a loop. When it makes a decision, it considers the current input and also what it has learned from the inputs it received previously.






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_e09e705a744c42cc8de229b5b737440f.png)






Below is side by side comparison of a regular Feed Forward Neural Network (MLP) and a Recurrent Neural Network (RNN). We can see that RNN is following a loop and learning from current and previous inputs.



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_cd688a706c6e47faba470e1eb7f86905.png)







### Applications of RNN

**Sentiment Classification**: This can be a task of simply classifying tweets into positive and negative sentiment. So here the input would be a tweet of varying lengths, while output is of a fixed type and size.


![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_e86f99ccbd2f4a648b146200b0cbba1d.png)


**Language Translation**: Imagine, we want to translate text from one language (English) to other language (French). Each language has its own semantics and would have varying lengths for the same sentence. So here the inputs as well as outputs are of varying lengths.





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_f97b044a50634fba9d74534dac875d6f.png)








**Image Captioning**: Here, let’s say we have an image for which we need a textual description. So we have a single input – the image, and a series or sequence of words as output. Here the image might be of a fixed size, but the output is a description of varying lengths








![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_a029389cac764a88b5b817b9ef90d780.png)









**SketchRNN**

https://magenta.tensorflow.org/assets/sketch_rnn_demo/index.html

This application learns to complete drawings. It’s pretty fun to play around with. Try it out!


You don’t need to do much here, just put a dot or add a line and the application would do the rest!



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_b98928ee8d8b462bba8a6ebf6b5bf756.png)




### Issues with Standard RNNs

* Gradient vanishing problems
* Exploding gradient problems
* Training an RNN is a comparatively difficult task.
* It cannot process very long sequences if using tanh or relu as an activation function.

## Long Short-Term Memory (LSTM)
* Long Short-Term Memory (LSTM) networks are a modified version of recurrent neural networks(RNNs), which makes it easier to remember past data in memory.
* The vanishing gradient problem of RNN is resolved here.
* Warning: The below image might look too complex at the moment. There’s nothing to fear, you’ll learn this in the next bootcamp.






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_00e9b01fdc2a495690bcd1e7ff32d31f.png)







## Gated Recurrent Unit (GRU)
* GRU (Gated Recurrent Unit) aims to solve the vanishing gradient problem which comes with a standard recurrent neural network.
* GRU can also be considered as a variation on the LSTM because both are designed similarly and, in some cases, produce equally excellent results.
* Another complex looking image alert! A gentle reminder: It gets easier when you understand it fully.









![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_2380a37ba4f547ed8e84101075134af0.png)








## Generative Adversarial Network (GAN)
Go to https://thispersondoesnotexist.com/ 

What do you see? A normal human being, right?

If you didn't figure out from the website name yet, the person you saw does not actually exist! It's an image generated by a Deep Learning technique called GAN. Each time you refresh the website, you'll see a completely new person. How cool is that?






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_c8c054c7a6eb45faa3a8779728005401.png)






Let us look at some examples to understand what a GAN and its variants are capable of:



![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_c605b62e49e7442b9372d3972d2a2d74.png)



* Given an image of the road, the network is able to fill in the details with objects such as cars etc.
* The network is able to convert a black & white image into colour.
* Given an aerial map, the network is able to find the roads in the image.
* It is also able to fill in the details of a photo, given the edges.

The network learns to generate from a training distribution through a 2-player game. The two entities are Generator and Discriminator.





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_0ae902212e084e4e9d205958a77909d4.png)




As you can identify from their names, a generator is used to generate real- looking images and the discriminator’s job is to identify which one is a fake. No need to get into their details at the moment. Just enjoy the glory of GANs!

## DeepFakes

Creating convincing image, audio and video hoaxes.










<iframe width="560" height="315" src="https://www.youtube.com/embed/cQ54GDm1eL0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>









Yes, the things in the above video were definitely not said by
former US President Barack Obama.

Once upon a time, the researchers were keen on creating DeepFakes.

Now, they are working on detecting them!

## Autoencoders
* Autoencoder learns how to efficiently compress and encode data then learns how to reconstruct the data back.
* It reduces data dimensions by learning how to ignore the noise in the data.




![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_969569dc5aa94a24b7fadcbe71dfbb40.png)




### Applications of Autoencoders


* Dimensionality Reduction
* Image Compression
* Image Denoising
* Feature Extraction
* Image generation
* Sequence to sequence prediction
* Recommendation system

### Additional Material (Optional)

A very basic introduction to implementing a Recurrent Neural Network:  
https://pythonprogramming.net/recurrent-neural-network-deep-learning-python-tensorflow-keras/

Implementing GANs in Tensorflow 2.0:  https://towardsdatascience.com/demystifying-gans-in-tensorflow-2-0-9890834ab3d9

Autoencoder with Tensorflow 2.0:  
https://www.geeksforgeeks.org/ml-autoencoder-with-tensorflow-2-0/

That’s just the tip of the iceberg. There are SO MANY more
neural networks out there!

Just to name a few more:
* Boltzmann Machine
* Bidirectional LSTMs
* Deep Belief Networks
* Radial Basis Function Neural Networks

Nope, you don’t need to dive into all of them at the moment. Go through the ones we’ve explained in the slides before, if you find some of them interesting, read about them and try to implement them.

If not, keep brushing up your skills on building MLP and CNN models. We’ll be covering advanced topics of Deep Learning like the ones mentioned in previous slides in the future Deep Learning Bootcamp.

Stay tuned to find out when that happens :)

### Slide Download Link

You can download the slides for this module [here](https://docs.google.com/presentation/d/1ZGrz6v_L7WDLf6onRw1S2SQQGSqhk8dy9bAuVJuZX9A/edit?usp=sharing).

### References
* https://www.analyticsvidhya.com/blog/2017/12/introduction-to-recurrent-neural-networks/
* https://builtin.com/data-science/recurrent-neural-networks-and-lstm
* https://towardsdatascience.com/generative-adversarial-networks-explained-34472718707a
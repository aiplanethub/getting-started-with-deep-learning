## Learning Objectives

* How do Computers see images?
* Computer Vision
* OpenCV

## How do Computers see images?

When we see this image, we can say, without even thinking, that this is an image of an adorable dog. Even an 8-year-old kid would not have any problem identifying the dog in the image.









![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_15a3c79a17424048917a6078da0cd966.png)










### Pixel
Have you ever wondered how a computer sees the same image?

A computer sees an image as 0s and 1s (binary digits).  
Pixel is the smallest unit in an image.






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_60303e4331d84b73bbd17d5e75244f2a.png)






Pixel data diagram. On the left is an image of Lincoln. In the center, the pixels are labeled 0–255, representing their brightness. On the right are the numbers themselves. What is this 0-255? It is RGB color combination values; we will learn about it soon.




![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_1b0d92842bab4a4eb106ba575dc2a9cb.png)





The ear of the animal has been zoomed in to show the pixel of an image.

### Channels

Computers are unable to recognize or look at images the way we humans would. So, we would have to find a way to convert these images into numbers. There are two common ways to do this when it comes to Image Processing:
1. **Greyscale** - A range of grey shades from white to black.
When using the Greyscale, the computer assigns each pixel a value (in numbers) based on its level of darkness.
2. **RGB Values** - A combination of red, green, and blue.
Once the color is given an RGB Value, the computer extracts that value from each pixel and puts the results in an array.

Each pixel contains a different number of channels. If it is a grayscale image, it has only one channel, whereas if it is a colored image, it contains three channels: red, green, and blue.




<p float="left" align='center'>
<img src = "https://dphi-live.s3.amazonaws.com/media_uploads/image_fff853435a574068927daaf08569f15c.png" width="100" /> <img src = "https://dphi-live.s3.amazonaws.com/media_uploads/image_392006567fce44e0b69258d1f9dc400e.png" width="100" />
</p>













As shown in the above representation of a digital colored image, each pixel channel has a value between 0 and 255.

### Understanding Color Images

For any color image in RGB format, there are three primary channels – Red, green and blue. How it works is pretty simple.

A matrix is formed for every primary color, and later these matrices combine to provide a Pixel value for the individual R, G, and B colors.

Consider the following image:





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_5b6aa9091df94fde89643e97c2842dbe.png)






Note: Images with 4, 5, or more channels also exist. An image can actually have up to 56 channels.

For example, images in sophisticated graphics editing use four channels: three channels for RGB plus an extra alpha or "a" channel.

Also, a CMYK image has four channels: cyan, magenta, yellow, and key (black).

When we say three channels, we consider RGB-type images.

### Image Representation

Images are usually represented as Height x Width x #Channels, where #Channels is 3 for RGB images and 1 for grayscale images.

Sometimes you see Width x Height x #Channels, but the third
dimension is the "channels."

The size of the image in the previous slide can be calculated as
B x A x 3.

Can you now understand why? (# means the number of something)





<iframe width="560" height="315" src="https://www.youtube.com/embed/LLAgPtpZth8?start=14" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>









The next question is, how can we say the image contains a picture of a dog?

Just reading the image is useless if it cannot understand what it means or if it cannot describe what the image is about and what it contains. This is where machine learning comes in.

A machine (or a computer) can be taught how to understand an image and say what the image contains. This is an example of machine learning teaching a computer to understand and describe an image. It is similar to how we teach kids to identify different alphabets or differentiate between an apple and a banana by showing examples of each case. This is exactly how a computer learns to identify objects in an image.

Like humans have different skills, and one of the skills is to identify an object in an image (a dog in the above image), computers have machine learning models, which can be thought of as a skill, to perform the same task. As humans need to be trained to perform a particular skill, computers also need to train the machine learning model.

In both cases, training happens using examples. Similar to how a kid is taught to identify an apple, a machine learning model can be taught how to identify an apple in an image by giving several images that contain an apple. From these example images, the model learns the features of an apple, like its shape and color. Now when a new image of an apple is presented to this computer with this model, it can use what it had learned about apples earlier and identify that this new image also contains an apple.

### How we teach computers to understand pictures
[In this amazing TED Talk](https://www.youtube.com/watch?v=40riCqvRoMs), Fei Fei Li - the co-director of the Stanford Institute for Human-Centered Artificial Intelligence, talks about the [ImageNet Dataset](https://image-net.org/) - a large dataset of over 14 million images, designed by academics intended for computer vision research that she created with fellow researchers.

The video dates back to 5 years ago but is still relevant today. ImageNet has played an important role in the advancement of computer vision. It is useful for many computer vision applications and is one of the most popular datasets for Computer Vision to date.

She also talks about the Convolutional Neural Networks and their crucial role in this domain. We will be learning more about CNN through a session recording soon.

## Computer Vision

Computer vision, often abbreviated as CV, is a field of artificial intelligence that trains computers to interpret and understand the visual world.

Breaking it down into its constituent words, Computer Vision = giving vision to the computers.

Using digital images from cameras and videos and deep learning models, machines can accurately identify and classify objects — and then react to what they "see."

Computer Vision is just one of the many applications of Deep Learning.

The goal of computer vision is to understand the content of digital images. Typically, this involves developing methods that attempt to reproduce the capability of human vision.

### How ML and DL revolutionized Computer Vision
Machine learning helped solve many challenging problems for classical software development tools and approaches. For instance, years ago, machine learning engineers were able to create software that could predict breast cancer survival windows better than human experts. However, building the software's features required the efforts of dozens of engineers and breast cancer experts and took a lot of time to develop.

Deep learning provided a fundamentally different approach to doing machine learning. Deep learning relies on neural networks, a general-purpose function that can solve any problem representable through examples. When you provide a neural network with many labeled examples of a specific kind of data, it'll be able to extract common patterns between those examples and transform them into a mathematical equation that will help classify future pieces of information.






![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_b9686f5367ce4b8b8e6585b767f2b8d9.png)







_Image source: zbigatron_

### DL - The star of Computer Vision
Deep learning is a very effective method for doing computer vision. In most cases, creating an excellent deep learning algorithm comes down to gathering a large amount of labeled training data and tuning the parameters such as the type and number of layers of neural networks and training epochs. Compared to previous types of machine learning, deep learning is easier and faster to develop and deploy.

Most current computer vision applications such as cancer detection, self-driving cars, and facial recognition use deep learning. Thanks to availability and advances in hardware and cloud computing resources, deep learning and deep neural networks have moved from the conceptual realm into practical applications.

### Applications Of Computer Vision

#### CV In Self-Driving(Autonomous) Cars

Computer vision enables self-driving cars to make sense of their surroundings. Cameras capture video from different angles around the car and feed it to computer vision software, which then processes the images in real-time to find the extremities of roads, read traffic signs, and detect other cars, objects, and pedestrians. The self-driving car can then steer its way on streets and highways, avoid hitting obstacles, and (hopefully) safely drive its passengers to their destination.




![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_1b5683c870c644739a86e6456a05efb5.png)







#### CV In Facial Recognition

Computer vision also plays an important role in facial recognition applications, enabling computers to match images of people's faces to their identities. Computer vision algorithms detect facial features in images and compare them with databases of face profiles. Consumer devices use facial recognition to authenticate the identities of their owners. Social media apps use facial recognition to detect and tag users. Law enforcement agencies also rely on facial recognition technology to identify criminals in video feeds.





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_e154582e549d45c59bbf0485fa3fb2b0.png)





#### CV In Healthcare

Computer vision has also been an important part of advances in health tech. Computer vision algorithms can help automate tasks such as detecting cancerous moles in skin images or finding symptoms in x-ray and MRI scans.








![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_5fed22bbb72240789b7f676307bec988.png)










### Computer Vision Tasks

Many popular computer vision applications involve trying to recognize things in photographs; for example:
* Object Classification: What broad category of object is in this photograph?
* Object Identification: Which type of a given object is in this photograph?
* Object Verification: Is the object in the photograph?
 * Object Detection: Where are the objects in the photograph?
 * Object Landmark Detection: What are the key points for the object in the photograph?
* Object Segmentation: What pixels belong to the object in the image?
* Object Recognition: What objects are in this photograph, and where are they?





![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_59f09a725d004678af029b0305917594.png)





Outside of just recognition, other methods of analysis include:

* Video motion analysis uses computer vision to estimate the velocity of objects in a video or the camera itself.
* In image segmentation, algorithms partition images into multiple sets of views.
* Scene reconstruction creates a 3D model of a scene inputted through images or video.
* Image restoration removes noise such as blurring from photos using Machine Learning based filters.

Any other application that involves understanding pixels through software can safely be labeled as computer vision.

Stating these tasks tackled by Computer Vision is not to overwhelm you but to introduce you to the immense capabilities Computer Vision holds.

## Basics of OpenCV and image processing


### What is OpenCV?


![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_b9bd251cd13a40878ab9b37c96850a38.png)




OpenCV (Open Source Computer Vision) is a library with functions mainly aimed at real-time computer vision. OpenCV supports Deep Learning frameworks like Caffe, Tensorflow, and Torch/PyTorch.

### Role of OpenCV in a computer vision project
* OpenCV is not used to train the neural networks—you should do that with a framework like TensorFlow or PyTorch and then export the model to run in OpenCV.
* OpenCV is used to take a trained neural network model, prepare and preprocess images for it, apply it to the images, and output results. You can also combine neural networks with other computer vision algorithms available in OpenCV.

### OpenCV Applications
* Detecting and recognizing faces
* Identifying objects
* Classifying human actions in videos
* Tracking camera movements
* Tracking moving objects
* Extracting 3D models of objects
* Producing 3D point clouds from stereo cameras
* Stitching images together to produce an image of a scene
* Finding similar images from an image database
* Removing red eyes from images
* Following eye movements
* Recognizing scenery by adding markers to enable augmented reality (AR)

And many more.

### Colour images in OpenCV

* OpenCV color images in the RGB (Red, Green, Blue) color space have a 3-tuple associated with each pixel: (B, G, R).
* Notice the ordering is BGR rather than RGB. This is because when OpenCV was first developed many years ago, the standard was BGR order. Over the years, the standard has become RGB, but OpenCV maintains this "legacy" BGR order to ensure no existing code breaks.

### Installing OpenCV
Before you can start learning OpenCV, you must install the OpenCV library on your system.
* If you are working on a Jupyter notebook on your device, you can
install OpenCV with:  
`pip install opencv-python`
* Colab users don't need to worry about this. OpenCV is installed
by default in Google Colab.

### Basic OpenCV Operations in practice
* The following notebook elaborates on the most commonly used
commands in OpenCV: https://github.com/dphi-official/Deep_Learning_Bootcamp/blob/master/OpenCV/DL_Day12_OpenCV.ipynb

### Slide Download Link
You can download the slides for this module from [here](https://docs.google.com/presentation/d/1h0Vw2h_HISqP4Di9DCSk-A_wwIgGtQf-j4ZBJJnSuJ0/edit?usp=sharing).

### References
* https://towardsdatascience.com/how-does-computer-understand-images-c1566d4537bf
* https://towardsdatascience.com/everything-you-ever-wanted-to-know-about-computer-vision-heres-a-look-why-it-s-so-awesome-e8a58dfb641e
* https://www.pyimagesearch.com/2018/07/19/opencv-tutorial-a-guide-to-learn-opencv/
* https://www.edureka.co/blog/python-opencv-tutorial/
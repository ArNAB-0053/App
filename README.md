# Groot
Detects diseases on a plant leaf.
# Welcome to the Groot wiki!

This repository includes the project of a leaf disease detection system named **"Groot"**

## Introduction-

If you just focus on the needs of human survival, there are basically four main things-
* Food
* shelter
* air 
* water

Today we are going to solve a silly problem yet a big solution. Its the most underrated thing that we humans just ignore. We just ignore the fact of its existence and a huge impact is faced by us every year. Yet this problem has been under existence before every sapiens or homo sapiens existence!!

If you can't guess it by now, then let me take you to the journey of the most silly problem with a "Groot" Solution!!!


## **Problem Statement-**

The main problem that we have given hints above is basically the diseases that occur in the plant and visible through our eyes on the leaf.
### So what's the problem in that??
There are many problems, we as humans can suffer if we negotiate this topic. 
* **Yield destruction-** 

As we know that India is one of the largest producer of crops around the globe. Our country yields and exports many vegetables and farm products to satisfy the needs of the world. One-third of our total population are in the primary sectors(The producing sector like- agriculture,fish-farming,etc). But after all this, we also face problems related to production every year. Isn't this a topic to discuss or isn't it a topic to be aware of and make farmers or the citizens to study about this?

India is a developing nation and a growing nation have to feed its citizen and to feed its growing population we need to grow the yield every year. But the statistics every year is different saying that "Nearly 20%-40% of the total yield is being destroyed every year", the reason to this statement has always been the climate change and less rain or flood situation throughout the country. But one of the basic problem that even the farmers negotiate or they are not aware about it or they don't know the solution to it...
"It is the disease of a plant". 

* **Allergies through Pathogens-**

You'd have seen people complaining about some allergies which basically occurs during specififc seasons(like- spring, monsoon,etc). This is basically due to some presence of pollens and pathogens in the air. But where do these come from? They are basically the output of the diseases on plants which travel through air. Plant diseases not only destroy the crop yields but effects human health too. These conditions can be very serious considering the stages.
 
* **Further evolution of diseases-**

In 2020, we recently faced a pandemic that was caused through a disruption in nature and the unknowing characteristic behaviour of a human being. Considering the evolving nature of everything in the universe we can expect a much more great pandemic due to these neglections. To prevent this situation to appear again, we need some solutions, some ideas to minimise the problem.


# **So what is the Solution?**

There are many solutions to it which are-
* Make people aware and make them study about this basic topic. Every problems basic solution is to make everyone aware about the problem and if we are aware abbout it then we can think and create new ideas to minimise it. There's always a saying that a problem with silly solutions are much better than no solution at all.

* If we are able to detect what is the type of disease that is growing on the plant then we can minimise it by producing some medicines or chemicals that can reduce it and doesn't alter the plants growth. If we can come up with these solutions we can make the production more and there will never be a problem anywhere related to food scarcity.

* The third way is to create a technology that will be user-friendly and be easily understandable by anyone. As we know that as we humans are evolving we are much more dependent on the smart devices and anyone can learn anything using these devices and can be an opportunity creator or can be a minimiser.

#What's our Approach?

So our approach is to design a Machine learning model that can use deep learning to detect the patterns fromed on the leaf surface and identify the type of disease from the dataset provided.

## **But how can we do it?**

Before studying the diseases, we have to know what pattern do they follow. 
*For example a leaf have some white powdery texture on its surface 
![image](https://user-images.githubusercontent.com/65272042/230682923-96c9d375-ffe9-4491-b3b1-5aad83e4e63e.png)
Then we can say that the above leaf is suffering from a disease called "**Powdery Mildew**".Just like this, if the leaf have some brown spots growing on it
![image](https://user-images.githubusercontent.com/65272042/230683402-65cb289e-e9c9-4fb1-8e3a-fd3bd5690c0e.png) 
![image](https://user-images.githubusercontent.com/65272042/230684770-a63ab721-cf0b-45ce-8905-74ca30a0bf85.png)

But there's a difference between these two pictures and those brown spots, the 1st picture signifies a disease called "**Rust**" in plants and the 2nd picture signifies "**Blight**". These two diseases are both fungal diseases but they both have different characteristics and solutions to minimise it.

These patterns have been the main reason to develop a model that can preprocess the image and can be trained in such a way that it can give the required results. The dataset has been made by capturing thousands of pictures of each disease on a specified leaf. Such huge amount of data made our model more accurate with accuracy percentage of "**65.76%**".

# **The data we are working on-**

![image](https://user-images.githubusercontent.com/65272042/230705790-5c9272a2-a60d-4593-b67e-88ddb71723fc.png)
The above graphical evaluation of data is of Loss vs val_loss. As we can see that to lines or functions tends to meet each other at some points. Just the thing that we have to remember is the more closer those two lines are the more accurate our predictions will be.

Deep learning has 4 basic stages to design a model-
*define/create a model
*start training/ fit model
*evaluation of the model 
*making predictions

The stage on which we are now is the third stage when the model is trained and now just we have to wait and watch for the code to run and evaluate itself and give its accuracy percentage.

![image](https://user-images.githubusercontent.com/65272042/230706068-8925c5c0-f906-45bb-b290-56b50202b7b0.png)

The above graph represent the evaluation between the accuracy and the val_accuracy. From which we will get the exact percentage of how much our model is capable to make predictions. Here we can see that the lines are again seem to meet together at some point. Thus, we can conclude that our model is trained and much more accurate.
 
# Drawbacks-

The basic drawback in our model that we can see is by again looking back at the graphical data. In that data we are able to see that the lines are crossing each other which can give a miscellaneous results sometime and can alter through the training model in making wrong predictions.
Our main goal is to make the model more accurate but training in such a way that no wrong predictions are made.

![faultloss](https://user-images.githubusercontent.com/65272042/230706546-ce1014b4-1482-4ca5-9f66-9284e352ec55.jpg)
![faultacc](https://user-images.githubusercontent.com/65272042/230706670-bc986aaf-dcac-4c1a-9e1a-00794c139675.jpg)

In the above graphs we can se those hazards where there are chances of high data losses and miss predictions.So these are the minor drawbacks that we have to resolve to make our model work smoothly.

# **A cute little Groot appeared-**

Enough talking about the diseases and stats of our machine learning model. Now let me take you through the journey of our littel android applications interface. The interface is clean and simple with a root logo. For now our application have the main page on which our Model would be working. 

![image](https://user-images.githubusercontent.com/65272042/230707096-83c1bc92-286d-4613-82c8-32d538f9e801.png)
This page is very simple and just have two backend operations to take a picture through mobile phones camera or the gallery. When the input is taken then that image is forwarded to our pre trained model and the model indicates which leaf it is and whether the leaf is healthy or diseased and if it is diseased then what kind of disease it have.  

# **Groot(0.1.0)**

In the testing face we faced many problems regarding the accuracy and the predictions. So the approach of our machine learning model got divided into three parts-
* Creation of model and training the model
* loading the model and doing the predictions
* Converting the file into tflite extension to use it in the application.

First, we minimised and balanced the amount of images of dataset from each class(set to 100). Then we started training the model and the architecture we used was basically CNN(Convolutional Neural Network). 
We used 5 layers namely-
* input layer
* Convolutional Layer
* Pooling layer
* Flatten
* Dense layer

![image](https://user-images.githubusercontent.com/65272042/230756435-ff94206b-706c-4a8d-8917-fcdf8e0703f8.png)

The code for architecture in our program looked like this-

![Screenshot 2023-04-09 111237](https://user-images.githubusercontent.com/65272042/230756528-2fbdd8f6-a7fc-41b1-b836-4046d4008bb4.jpg)

Then we trained the model and saved it.

Now it was the time for predicition and we load the model in a different notebook and started the evaluation. 

![bcw](https://user-images.githubusercontent.com/65272042/230757316-efbe5fde-d408-4bed-bf42-cc253bfa736f.jpg)

After all the prediction, the accuracy was-
![Screenshot 2023-04-09 113347](https://user-images.githubusercontent.com/65272042/230757307-49e3f011-2a02-4ed6-9ee2-9e95958ad79d.jpg)

Thus the accuracy was increased from the earlier version and now it was the time to use it as a feature in the application.

Then we Coverted this file into a tflite extension for the use in android.
![Screenshot 2023-04-09 114447](https://user-images.githubusercontent.com/65272042/230757705-b90b9909-14b5-4df7-bcff-8944e5e6531b.jpg)

Introducing the New Groot-

![image](https://user-images.githubusercontent.com/65272042/230757413-751393f5-7342-473f-aaab-1b0fa942d9b0.png)

![image](https://user-images.githubusercontent.com/65272042/230757452-4f893830-9806-4ae5-84d2-2e94c704a1c6.png)

![image](https://user-images.githubusercontent.com/65272042/230757488-ae029cbb-597e-4a81-9b55-53cb41ea933b.png)

## *Future Instances-*
* In future we will try to make a page for the application where the solution related to the specified disease will be given 
* A monitoring system that can monitor the growth of a plant and can detect even a single anomaly. 
* A section for agriculutural news and some articles related to the modern methods of agriculture.

# *Conclusion-*

So the ideas that we proposed has came to an end, but more things have to be done in future. So that our future generations can learn, care and be precautious about everything that is present in future.
Atlast now we know what hazards silly problems can create if we neglected it.

If we decide to save our nature first, we can create our own Utopia.
